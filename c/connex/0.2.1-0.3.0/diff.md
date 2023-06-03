# Comparing `tmp/connex-0.2.1.tar.gz` & `tmp/connex-0.3.0.tar.gz`

## Comparing `connex-0.2.1.tar` & `connex-0.3.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 connex-0.2.1/connex/__init__.py
--rw-r--r--   0        0        0    35145 2020-02-02 00:00:00.000000 connex-0.2.1/connex/_network.py
--rw-r--r--   0        0        0    46899 2020-02-02 00:00:00.000000 connex-0.2.1/connex/_plasticity.py
--rw-r--r--   0        0        0     1274 2020-02-02 00:00:00.000000 connex-0.2.1/connex/_utils.py
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 connex-0.2.1/connex/nn/__init__.py
--rw-r--r--   0        0        0     3062 2020-02-02 00:00:00.000000 connex-0.2.1/connex/nn/_dense_mlp.py
--rw-r--r--   0        0        0     2526 2020-02-02 00:00:00.000000 connex-0.2.1/connex/nn/_mlp.py
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 connex-0.2.1/connex/nn/_utils.py
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 connex-0.2.1/.gitignore
--rw-r--r--   0        0        0    11356 2020-02-02 00:00:00.000000 connex-0.2.1/LICENSE
--rw-r--r--   0        0        0     3781 2020-02-02 00:00:00.000000 connex-0.2.1/README.md
--rw-r--r--   0        0        0     1119 2020-02-02 00:00:00.000000 connex-0.2.1/pyproject.toml
--rw-r--r--   0        0        0    17782 2020-02-02 00:00:00.000000 connex-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 connex-0.3.0/connex/__init__.py
+-rw-r--r--   0        0        0    33027 2020-02-02 00:00:00.000000 connex-0.3.0/connex/_network.py
+-rw-r--r--   0        0        0    46899 2020-02-02 00:00:00.000000 connex-0.3.0/connex/_plasticity.py
+-rw-r--r--   0        0        0     1459 2020-02-02 00:00:00.000000 connex-0.3.0/connex/_utils.py
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 connex-0.3.0/connex/nn/__init__.py
+-rw-r--r--   0        0        0     3062 2020-02-02 00:00:00.000000 connex-0.3.0/connex/nn/_dense_mlp.py
+-rw-r--r--   0        0        0     2526 2020-02-02 00:00:00.000000 connex-0.3.0/connex/nn/_mlp.py
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 connex-0.3.0/connex/nn/_utils.py
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 connex-0.3.0/.gitignore
+-rw-r--r--   0        0        0    11356 2020-02-02 00:00:00.000000 connex-0.3.0/LICENSE
+-rw-r--r--   0        0        0     3677 2020-02-02 00:00:00.000000 connex-0.3.0/README.md
+-rw-r--r--   0        0        0     1148 2020-02-02 00:00:00.000000 connex-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0    17707 2020-02-02 00:00:00.000000 connex-0.3.0/PKG-INFO
```

### Comparing `connex-0.2.1/connex/_network.py` & `connex-0.3.0/connex/_network.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 from typing import Any, Callable, Dict, List, Mapping, Optional, Sequence, Tuple, Union
 
 import jax.nn as jnn
 import jax.numpy as jnp
 import jax.random as jr
 import networkx as nx
 import numpy as np
-from equinox import filter_jit, Module, static_field, tree_at
+from equinox import filter_jit, Module, static_field
 from jax import Array, jit, lax, vmap
 
-from ._utils import _identity, _invert_dict, DiGraphLike
+from ._utils import _identity, _invert_dict, _keygen, DiGraphLike
 
 
 class NeuralNetwork(Module):
     """A neural network whose structure is specified by a DAG."""
 
     _weights_and_biases: List[Array]
     _hidden_activation: Callable
@@ -177,19 +177,15 @@
             use_neuron_self_attention,
             use_adaptive_activations,
             key,
         )
         self._set_dropout_p_initial(dropout_p)
 
     @filter_jit
-    def __call__(
-        self,
-        x: Array,
-        key: Optional[jr.PRNGKey] = None,
-    ) -> Array:
+    def __call__(self, x: Array, *, key: Optional[jr.PRNGKey] = None) -> Array:
         """The forward pass of the network.
         Neurons are "fired" in topological batch order -- see Section 2.2 of
 
         ??? cite
 
             [Directed Acyclic Graph Neural Networks](https://arxiv.org/abs/2101.07965)
             ```bibtex
@@ -203,26 +199,27 @@
             ```
 
         **Arguments**:
 
         - `x`: The input array to the network for the forward pass. The individual
             values will be written to the input neurons in the order passed in during
             initialization.
-        - `key`: A `jax.random.PRNGKey` used for dropout. Must be provided, even if all
-            dropout probabilities are 0.
+        - `key`: A `jax.random.PRNGKey` used for dropout. Optional, keyword-only
+            argument. If `None`, a key will be generated using the current time.
 
         **Returns**:
 
         The result array from the forward pass. The order of the array elements will be
         the order of the output neurons passed in during initialization.
         """
         # Neuron value array, updated as neurons are "fired"
         values = jnp.zeros((self._num_neurons,))
 
         # Dropout
+        key = _keygen() if key is None else key
         rand = jr.uniform(key, self._dropout_array.shape, minval=0, maxval=1)
         dropout_mask = jnp.greater(rand, self._dropout_array)
 
         # Set input values
         values = values.at[self._input_neurons_id].set(
             x * dropout_mask[self._input_neurons_id]
         )
@@ -740,65 +737,14 @@
         self._dropout_array = dropout_array
         self._dropout_dict = dropout_dict
 
     #####################################################
     ################## Public methods ###################  # noqa: E266
     #####################################################
 
-    def set_dropout_p(
-        self, dropout_p: Union[float, Mapping[Any, float]]
-    ) -> "NeuralNetwork":
-        """Set the per-neuron dropout probabilities.
-
-        **Arguments:**
-
-        - `dropout_p`: Either a float or mapping from neuron (`Any`) to float. If a
-            single float, all hidden neurons will have that dropout probability, and
-            all input and output neurons will have dropout probability 0 by default.
-            If a `Mapping`, it is assumed that `dropout_p` maps a neuron to its dropout
-            probability, and all unspecified neurons will retain their current dropout
-            probability.
-
-        **Returns:**
-
-        A copy of the current network with dropout probabilities as specified.
-        The original network (including unspecified dropout probabilities) is left
-        unchanged.
-        """
-
-        def update_dropout_probabilities():
-            if isinstance(dropout_p, float):
-                hidden_dropout = {neuron: dropout_p for neuron in self._hidden_neurons}
-                input_output_dropout = {
-                    neuron: 0.0 for neuron in self._input_neurons + self._output_neurons
-                }
-                return {**hidden_dropout, **input_output_dropout}
-            else:
-                assert isinstance(dropout_p, Mapping)
-                for n, d in dropout_p.items():
-                    if n not in self._graph.nodes:
-                        raise ValueError(f"'{n}' is not present in the network.")
-                    if not isinstance(d, float):
-                        raise TypeError(f"Invalid dropout value of {d} for neuron {n}.")
-                    return {**self._dropout_dict, **dropout_p}
-
-        dropout_dict = update_dropout_probabilities()
-        dropout_array = jnp.array(
-            [dropout_dict[neuron] for neuron in self._topo_sort], dtype=float
-        )
-
-        assert jnp.all(jnp.greater_equal(dropout_array, 0))
-        assert jnp.all(jnp.less_equal(dropout_array, 1))
-
-        return tree_at(
-            lambda network: (network._dropout_dict, network._dropout_array),
-            self,
-            (dropout_dict, dropout_array),
-        )
-
     def to_networkx_weighted_digraph(self) -> nx.DiGraph:
         """Returns a `networkx.DiGraph` represention of the network with neuron weights
         saved as edge attributes."""
 
         def _get_edge_attributes():
             edge_attrs = {}
             for neuron, inputs in self._adjacency_dict_inv.items():
```

### Comparing `connex-0.2.1/connex/_plasticity.py` & `connex-0.3.0/connex/_plasticity.py`

 * *Files identical despite different names*

### Comparing `connex-0.2.1/connex/_utils.py` & `connex-0.3.0/connex/_utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import time
 import typing
 from collections import defaultdict
 from typing import Any, Dict, List
 
 import jax.nn as jnn
+import jax.random as jr
 
 
 # Documentation helpers.
 
 
 def _identity(x):
     return x
@@ -52,7 +53,15 @@
 
 
 def _edges_to_adjacency_dict(edges):
     adjacency_dict = defaultdict(list)
     for u, v in edges:
         adjacency_dict[u].append(v)
     return dict(adjacency_dict)
+
+
+def _keygen():
+    curr_time = time.time()
+    curr_time = str(curr_time).replace(".", "")
+    seed = int(curr_time)
+    key = jr.PRNGKey(seed)
+    return key
```

### Comparing `connex-0.2.1/connex/nn/_dense_mlp.py` & `connex-0.3.0/connex/nn/_dense_mlp.py`

 * *Files identical despite different names*

### Comparing `connex-0.2.1/connex/nn/_mlp.py` & `connex-0.3.0/connex/nn/_mlp.py`

 * *Files identical despite different names*

### Comparing `connex-0.2.1/LICENSE` & `connex-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `connex-0.2.1/README.md` & `connex-0.3.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -65,37 +65,35 @@
 
 # Initialize the optimizer
 optim = optax.adam(1e-3)
 opt_state = optim.init(eqx.filter(network, eqx.is_array))
 
 # Define the loss function
 @eqx.filter_value_and_grad
-def loss_fn(model, x, y, keys):
-    preds = jax.vmap(model)(x, keys)
+def loss_fn(model, x, y):
+    preds = jax.vmap(model)(x)
     return jnp.mean((preds - y) ** 2)
 
 # Define a single training step
 @eqx.filter_jit
-def step(model, opt_state, x, y, keys):
-    loss, grads = loss_fn(model, x, y, keys)
+def step(model, opt_state, x, y):
+    loss, grads = loss_fn(model, x, y)
     updates, opt_state = optim.update(grads, opt_state, model)
     model = eqx.apply_updates(model, updates)
     return model, opt_state, loss
 
 # Toy data
 x = jnp.expand_dims(jnp.linspace(0, 2 * jnp.pi, 250), 1)
 y = jnp.hstack((jnp.cos(x), jnp.sin(x)))
 
 # Training loop
 n_epochs = 500
 key = jr.PRNGKey(0)
 for epoch in range(n_epochs):
-    *keys, key = jr.split(key, x.shape[0] + 1)
-    keys = jnp.array(keys)
-    network, opt_state, loss = step(network, opt_state, x, y, keys)
+    network, opt_state, loss = step(network, opt_state, x, y)
     print(f"Epoch: {epoch + 1}   Loss: {loss}")
 ```
 
 Now suppose we wish to add connections 1 &rarr; 6 and 2 &rarr; 11, remove neuron 9, and set the dropout probability of all hidden neurons to 0.1:
 
 ```python
 # Add connections
```

### Comparing `connex-0.2.1/pyproject.toml` & `connex-0.3.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [project]
 name = "connex"
-version = "0.2.1"
-description = "Making neural networks more neural."
+version = "0.3.0"
+description = "Fine-grained, dynamic control of neural network topology in JAX."
 readme = "README.md"
-requires-python ="~=3.8"
+requires-python ="~=3.9"
 license = {file = "LICENSE"}
 authors = [
   {name = "Leonard Gleyzer", email = "lenny@lenn.ai"},
 ]
 keywords = ["jax", "neural-networks", "deep-learning"]
 classifiers = [
     "Development Status :: 3 - Alpha",
@@ -19,15 +19,15 @@
     "Natural Language :: English",
     "Programming Language :: Python :: 3",
     "Topic :: Scientific/Engineering :: Artificial Intelligence",
     "Topic :: Scientific/Engineering :: Information Analysis",
     "Topic :: Scientific/Engineering :: Mathematics",
 ]
 urls = {repository = "https://github.com/leonard-gleyzer/connex" }
-dependencies = ["equinox>=0.10.4", "jax>=0.4.4", "networkx>=0.3.0"]
+dependencies = ["equinox>=0.10.5", "jax>=0.4.4", "networkx>=0.3.0"]
 
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [tool.hatch.build]
 include = ["connex/*"]
```

### Comparing `connex-0.2.1/PKG-INFO` & `connex-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: connex
-Version: 0.2.1
-Summary: Making neural networks more neural.
+Version: 0.3.0
+Summary: Fine-grained, dynamic control of neural network topology in JAX.
 Project-URL: repository, https://github.com/leonard-gleyzer/connex
 Author-email: Leonard Gleyzer <lenny@lenn.ai>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -214,16 +214,16 @@
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Scientific/Engineering :: Mathematics
-Requires-Python: ~=3.8
-Requires-Dist: equinox>=0.10.4
+Requires-Python: ~=3.9
+Requires-Dist: equinox>=0.10.5
 Requires-Dist: jax>=0.4.4
 Requires-Dist: networkx>=0.3.0
 Description-Content-Type: text/markdown
 
 <h1 align='center'>Connex</h1>
 
 Connex is a [JAX](https://github.com/google/jax) library built on [Equinox](https://github.com/patrick-kidger/equinox) that allows for fine-grained, dynamic control of neural network topology. With Connex, you can
@@ -291,37 +291,35 @@
 
 # Initialize the optimizer
 optim = optax.adam(1e-3)
 opt_state = optim.init(eqx.filter(network, eqx.is_array))
 
 # Define the loss function
 @eqx.filter_value_and_grad
-def loss_fn(model, x, y, keys):
-    preds = jax.vmap(model)(x, keys)
+def loss_fn(model, x, y):
+    preds = jax.vmap(model)(x)
     return jnp.mean((preds - y) ** 2)
 
 # Define a single training step
 @eqx.filter_jit
-def step(model, opt_state, x, y, keys):
-    loss, grads = loss_fn(model, x, y, keys)
+def step(model, opt_state, x, y):
+    loss, grads = loss_fn(model, x, y)
     updates, opt_state = optim.update(grads, opt_state, model)
     model = eqx.apply_updates(model, updates)
     return model, opt_state, loss
 
 # Toy data
 x = jnp.expand_dims(jnp.linspace(0, 2 * jnp.pi, 250), 1)
 y = jnp.hstack((jnp.cos(x), jnp.sin(x)))
 
 # Training loop
 n_epochs = 500
 key = jr.PRNGKey(0)
 for epoch in range(n_epochs):
-    *keys, key = jr.split(key, x.shape[0] + 1)
-    keys = jnp.array(keys)
-    network, opt_state, loss = step(network, opt_state, x, y, keys)
+    network, opt_state, loss = step(network, opt_state, x, y)
     print(f"Epoch: {epoch + 1}   Loss: {loss}")
 ```
 
 Now suppose we wish to add connections 1 &rarr; 6 and 2 &rarr; 11, remove neuron 9, and set the dropout probability of all hidden neurons to 0.1:
 
 ```python
 # Add connections
```

