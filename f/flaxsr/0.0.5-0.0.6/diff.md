# Comparing `tmp/flaxsr-0.0.5.tar.gz` & `tmp/flaxsr-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flaxsr-0.0.5.tar", last modified: Fri Jun  2 13:53:12 2023, max compression
+gzip compressed data, was "flaxsr-0.0.6.tar", last modified: Sat Jun  3 08:57:01 2023, max compression
```

## Comparing `flaxsr-0.0.5.tar` & `flaxsr-0.0.6.tar`

### file list

```diff
@@ -1,39 +1,40 @@
-drwxrwxr-x   0 dslisleedh  (1007) dslisleedh  (1007)        0 2023-06-02 13:53:12.175251 flaxsr-0.0.5/
--rw-rw-r--   0 dslisleedh  (1007) dslisleedh  (1007)    11313 2023-05-12 09:22:40.000000 flaxsr-0.0.5/LICENSE
--rw-rw-r--   0 dslisleedh  (1007) dslisleedh  (1007)     1948 2023-06-02 13:53:12.175251 flaxsr-0.0.5/PKG-INFO
--rw-rw-r--   0 dslisleedh  (1007) dslisleedh  (1007)     1324 2023-06-02 13:51:10.000000 flaxsr-0.0.5/README.md
-drwxrwxr-x   0 dslisleedh  (1007) dslisleedh  (1007)        0 2023-06-02 13:53:12.175251 flaxsr-0.0.5/flaxsr/
--rw-rw-r--   0 dslisleedh  (1007) dslisleedh  (1007)      111 2023-05-17 15:18:45.000000 flaxsr-0.0.5/flaxsr/__init__.py
--rw-rw-r--   0 dslisleedh  (1007) dslisleedh  (1007)      661 2023-05-12 10:02:07.000000 flaxsr-0.0.5/flaxsr/_utils.py
-drwxrwxr-x   0 dslisleedh  (1007) dslisleedh  (1007)        0 2023-06-02 13:53:12.175251 flaxsr-0.0.5/flaxsr/layers/
--rw-rw-r--   0 dslisleedh  (1007) dslisleedh  (1007)      179 2023-05-12 09:22:40.000000 flaxsr-0.0.5/flaxsr/layers/__init__.py
--rw-rw-r--   0 dslisleedh  (1007) dslisleedh  (1007)     1651 2023-05-16 13:28:13.000000 flaxsr-0.0.5/flaxsr/layers/stochastic.py
--rw-rw-r--   0 dslisleedh  (1007) dslisleedh  (1007)     1673 2023-05-16 13:28:27.000000 flaxsr-0.0.5/flaxsr/layers/upscale.py
-drwxrwxr-x   0 dslisleedh  (1007) dslisleedh  (1007)        0 2023-06-02 13:53:12.175251 flaxsr-0.0.5/flaxsr/losses/
--rw-rw-r--   0 dslisleedh  (1007) dslisleedh  (1007)     1384 2023-06-02 13:50:17.000000 flaxsr-0.0.5/flaxsr/losses/__init__.py
--rw-rw-r--   0 dslisleedh  (1007) dslisleedh  (1007)     4806 2023-06-02 13:04:49.000000 flaxsr-0.0.5/flaxsr/losses/adversarial_losses.py
--rw-rw-r--   0 dslisleedh  (1007) dslisleedh  (1007)     2495 2023-06-02 12:29:07.000000 flaxsr-0.0.5/flaxsr/losses/perceptual_losses.py
--rw-rw-r--   0 dslisleedh  (1007) dslisleedh  (1007)     2229 2023-06-02 12:17:52.000000 flaxsr-0.0.5/flaxsr/losses/pixel_wise_losses.py
--rw-rw-r--   0 dslisleedh  (1007) dslisleedh  (1007)     3190 2023-06-02 13:06:59.000000 flaxsr-0.0.5/flaxsr/losses/utils.py
-drwxrwxr-x   0 dslisleedh  (1007) dslisleedh  (1007)        0 2023-06-02 13:53:12.175251 flaxsr-0.0.5/flaxsr/models/
--rw-rw-r--   0 dslisleedh  (1007) dslisleedh  (1007)      392 2023-06-02 11:31:44.000000 flaxsr-0.0.5/flaxsr/models/__init__.py
--rw-rw-r--   0 dslisleedh  (1007) dslisleedh  (1007)     3749 2023-05-12 09:48:06.000000 flaxsr-0.0.5/flaxsr/models/edsr.py
--rw-rw-r--   0 dslisleedh  (1007) dslisleedh  (1007)      922 2023-05-12 09:48:06.000000 flaxsr-0.0.5/flaxsr/models/espcn.py
--rw-rw-r--   0 dslisleedh  (1007) dslisleedh  (1007)     1138 2023-05-12 09:48:06.000000 flaxsr-0.0.5/flaxsr/models/fsrcnn.py
--rw-rw-r--   0 dslisleedh  (1007) dslisleedh  (1007)     6677 2023-05-12 09:48:06.000000 flaxsr-0.0.5/flaxsr/models/nafssr.py
--rw-rw-r--   0 dslisleedh  (1007) dslisleedh  (1007)      994 2023-05-12 09:48:06.000000 flaxsr-0.0.5/flaxsr/models/ncnet.py
--rw-rw-r--   0 dslisleedh  (1007) dslisleedh  (1007)     1078 2023-05-12 09:49:43.000000 flaxsr-0.0.5/flaxsr/models/srcnn.py
--rw-rw-r--   0 dslisleedh  (1007) dslisleedh  (1007)     4161 2023-06-02 11:35:45.000000 flaxsr-0.0.5/flaxsr/models/srgan.py
--rw-rw-r--   0 dslisleedh  (1007) dslisleedh  (1007)      954 2023-05-12 09:50:48.000000 flaxsr-0.0.5/flaxsr/models/vdsr.py
-drwxrwxr-x   0 dslisleedh  (1007) dslisleedh  (1007)        0 2023-06-02 13:53:12.175251 flaxsr-0.0.5/flaxsr/training/
--rw-rw-r--   0 dslisleedh  (1007) dslisleedh  (1007)      149 2023-06-01 05:21:42.000000 flaxsr-0.0.5/flaxsr/training/__init__.py
--rw-rw-r--   0 dslisleedh  (1007) dslisleedh  (1007)      503 2023-06-01 00:48:20.000000 flaxsr-0.0.5/flaxsr/training/train_states.py
--rw-rw-r--   0 dslisleedh  (1007) dslisleedh  (1007)     1345 2023-06-01 05:25:08.000000 flaxsr-0.0.5/flaxsr/training/train_step.py
-drwxrwxr-x   0 dslisleedh  (1007) dslisleedh  (1007)        0 2023-06-02 13:53:12.175251 flaxsr-0.0.5/flaxsr.egg-info/
--rw-rw-r--   0 dslisleedh  (1007) dslisleedh  (1007)     1948 2023-06-02 13:53:12.000000 flaxsr-0.0.5/flaxsr.egg-info/PKG-INFO
--rw-rw-r--   0 dslisleedh  (1007) dslisleedh  (1007)      745 2023-06-02 13:53:12.000000 flaxsr-0.0.5/flaxsr.egg-info/SOURCES.txt
--rw-rw-r--   0 dslisleedh  (1007) dslisleedh  (1007)        1 2023-06-02 13:53:12.000000 flaxsr-0.0.5/flaxsr.egg-info/dependency_links.txt
--rw-rw-r--   0 dslisleedh  (1007) dslisleedh  (1007)       46 2023-06-02 13:53:12.000000 flaxsr-0.0.5/flaxsr.egg-info/requires.txt
--rw-rw-r--   0 dslisleedh  (1007) dslisleedh  (1007)        7 2023-06-02 13:53:12.000000 flaxsr-0.0.5/flaxsr.egg-info/top_level.txt
--rw-rw-r--   0 dslisleedh  (1007) dslisleedh  (1007)       38 2023-06-02 13:53:12.175251 flaxsr-0.0.5/setup.cfg
--rw-rw-r--   0 dslisleedh  (1007) dslisleedh  (1007)      961 2023-06-02 13:52:56.000000 flaxsr-0.0.5/setup.py
+drwxrwxr-x   0 dslisleedh  (1007) dslisleedh  (1007)        0 2023-06-03 08:57:01.268914 flaxsr-0.0.6/
+-rw-rw-r--   0 dslisleedh  (1007) dslisleedh  (1007)    11313 2023-05-12 09:22:40.000000 flaxsr-0.0.6/LICENSE
+-rw-rw-r--   0 dslisleedh  (1007) dslisleedh  (1007)     2800 2023-06-03 08:57:01.268914 flaxsr-0.0.6/PKG-INFO
+-rw-rw-r--   0 dslisleedh  (1007) dslisleedh  (1007)     2176 2023-06-03 08:09:59.000000 flaxsr-0.0.6/README.md
+drwxrwxr-x   0 dslisleedh  (1007) dslisleedh  (1007)        0 2023-06-03 08:57:01.264914 flaxsr-0.0.6/flaxsr/
+-rw-rw-r--   0 dslisleedh  (1007) dslisleedh  (1007)      111 2023-05-17 15:18:45.000000 flaxsr-0.0.6/flaxsr/__init__.py
+-rw-rw-r--   0 dslisleedh  (1007) dslisleedh  (1007)      661 2023-05-12 10:02:07.000000 flaxsr-0.0.6/flaxsr/_utils.py
+drwxrwxr-x   0 dslisleedh  (1007) dslisleedh  (1007)        0 2023-06-03 08:57:01.268914 flaxsr-0.0.6/flaxsr/layers/
+-rw-rw-r--   0 dslisleedh  (1007) dslisleedh  (1007)      179 2023-05-12 09:22:40.000000 flaxsr-0.0.6/flaxsr/layers/__init__.py
+-rw-rw-r--   0 dslisleedh  (1007) dslisleedh  (1007)     1651 2023-05-16 13:28:13.000000 flaxsr-0.0.6/flaxsr/layers/stochastic.py
+-rw-rw-r--   0 dslisleedh  (1007) dslisleedh  (1007)     1673 2023-05-16 13:28:27.000000 flaxsr-0.0.6/flaxsr/layers/upscale.py
+drwxrwxr-x   0 dslisleedh  (1007) dslisleedh  (1007)        0 2023-06-03 08:57:01.268914 flaxsr-0.0.6/flaxsr/losses/
+-rw-rw-r--   0 dslisleedh  (1007) dslisleedh  (1007)     1647 2023-06-03 08:08:49.000000 flaxsr-0.0.6/flaxsr/losses/__init__.py
+-rw-rw-r--   0 dslisleedh  (1007) dslisleedh  (1007)     4806 2023-06-03 04:02:44.000000 flaxsr-0.0.6/flaxsr/losses/adversarial_losses.py
+-rw-rw-r--   0 dslisleedh  (1007) dslisleedh  (1007)     2506 2023-06-03 03:59:09.000000 flaxsr-0.0.6/flaxsr/losses/perceptual_losses.py
+-rw-rw-r--   0 dslisleedh  (1007) dslisleedh  (1007)     2230 2023-06-03 03:58:37.000000 flaxsr-0.0.6/flaxsr/losses/pixel_wise_losses.py
+-rw-rw-r--   0 dslisleedh  (1007) dslisleedh  (1007)     6448 2023-06-03 08:48:01.000000 flaxsr-0.0.6/flaxsr/losses/regularization_losses.py
+-rw-rw-r--   0 dslisleedh  (1007) dslisleedh  (1007)     3321 2023-06-03 08:38:58.000000 flaxsr-0.0.6/flaxsr/losses/utils.py
+drwxrwxr-x   0 dslisleedh  (1007) dslisleedh  (1007)        0 2023-06-03 08:57:01.268914 flaxsr-0.0.6/flaxsr/models/
+-rw-rw-r--   0 dslisleedh  (1007) dslisleedh  (1007)      392 2023-06-02 11:31:44.000000 flaxsr-0.0.6/flaxsr/models/__init__.py
+-rw-rw-r--   0 dslisleedh  (1007) dslisleedh  (1007)     3749 2023-05-12 09:48:06.000000 flaxsr-0.0.6/flaxsr/models/edsr.py
+-rw-rw-r--   0 dslisleedh  (1007) dslisleedh  (1007)      922 2023-05-12 09:48:06.000000 flaxsr-0.0.6/flaxsr/models/espcn.py
+-rw-rw-r--   0 dslisleedh  (1007) dslisleedh  (1007)     1138 2023-05-12 09:48:06.000000 flaxsr-0.0.6/flaxsr/models/fsrcnn.py
+-rw-rw-r--   0 dslisleedh  (1007) dslisleedh  (1007)     6677 2023-05-12 09:48:06.000000 flaxsr-0.0.6/flaxsr/models/nafssr.py
+-rw-rw-r--   0 dslisleedh  (1007) dslisleedh  (1007)      994 2023-05-12 09:48:06.000000 flaxsr-0.0.6/flaxsr/models/ncnet.py
+-rw-rw-r--   0 dslisleedh  (1007) dslisleedh  (1007)     1078 2023-05-12 09:49:43.000000 flaxsr-0.0.6/flaxsr/models/srcnn.py
+-rw-rw-r--   0 dslisleedh  (1007) dslisleedh  (1007)     4161 2023-06-02 11:35:45.000000 flaxsr-0.0.6/flaxsr/models/srgan.py
+-rw-rw-r--   0 dslisleedh  (1007) dslisleedh  (1007)      954 2023-05-12 09:50:48.000000 flaxsr-0.0.6/flaxsr/models/vdsr.py
+drwxrwxr-x   0 dslisleedh  (1007) dslisleedh  (1007)        0 2023-06-03 08:57:01.268914 flaxsr-0.0.6/flaxsr/training/
+-rw-rw-r--   0 dslisleedh  (1007) dslisleedh  (1007)      149 2023-06-01 05:21:42.000000 flaxsr-0.0.6/flaxsr/training/__init__.py
+-rw-rw-r--   0 dslisleedh  (1007) dslisleedh  (1007)      503 2023-06-01 00:48:20.000000 flaxsr-0.0.6/flaxsr/training/train_states.py
+-rw-rw-r--   0 dslisleedh  (1007) dslisleedh  (1007)     1345 2023-06-03 08:06:45.000000 flaxsr-0.0.6/flaxsr/training/train_step.py
+drwxrwxr-x   0 dslisleedh  (1007) dslisleedh  (1007)        0 2023-06-03 08:57:01.268914 flaxsr-0.0.6/flaxsr.egg-info/
+-rw-rw-r--   0 dslisleedh  (1007) dslisleedh  (1007)     2800 2023-06-03 08:57:01.000000 flaxsr-0.0.6/flaxsr.egg-info/PKG-INFO
+-rw-rw-r--   0 dslisleedh  (1007) dslisleedh  (1007)      784 2023-06-03 08:57:01.000000 flaxsr-0.0.6/flaxsr.egg-info/SOURCES.txt
+-rw-rw-r--   0 dslisleedh  (1007) dslisleedh  (1007)        1 2023-06-03 08:57:01.000000 flaxsr-0.0.6/flaxsr.egg-info/dependency_links.txt
+-rw-rw-r--   0 dslisleedh  (1007) dslisleedh  (1007)       46 2023-06-03 08:57:01.000000 flaxsr-0.0.6/flaxsr.egg-info/requires.txt
+-rw-rw-r--   0 dslisleedh  (1007) dslisleedh  (1007)        7 2023-06-03 08:57:01.000000 flaxsr-0.0.6/flaxsr.egg-info/top_level.txt
+-rw-rw-r--   0 dslisleedh  (1007) dslisleedh  (1007)       38 2023-06-03 08:57:01.268914 flaxsr-0.0.6/setup.cfg
+-rw-rw-r--   0 dslisleedh  (1007) dslisleedh  (1007)      960 2023-06-03 08:56:02.000000 flaxsr-0.0.6/setup.py
```

### Comparing `flaxsr-0.0.5/LICENSE` & `flaxsr-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `flaxsr-0.0.5/flaxsr/_utils.py` & `flaxsr-0.0.6/flaxsr/_utils.py`

 * *Files identical despite different names*

### Comparing `flaxsr-0.0.5/flaxsr/layers/stochastic.py` & `flaxsr-0.0.6/flaxsr/layers/stochastic.py`

 * *Files identical despite different names*

### Comparing `flaxsr-0.0.5/flaxsr/layers/upscale.py` & `flaxsr-0.0.6/flaxsr/layers/upscale.py`

 * *Files identical despite different names*

### Comparing `flaxsr-0.0.5/flaxsr/losses/__init__.py` & `flaxsr-0.0.6/flaxsr/losses/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -20,19 +20,26 @@
     LeastSquareDiscriminatorLoss as LeastSquareDiscriminatorLoss,
     LeastSquareGeneratorLoss as LeastSquareGeneratorLoss,
     relativistic_discriminator_loss as relativistic_discriminator_loss,
     relativistic_generator_loss as relativistic_generator_loss,
     RelativisticDiscriminatorLoss as RelativisticDiscriminatorLoss,
     RelativisticGeneratorLoss as RelativisticGeneratorLoss,
 )
+from .regularization_losses import (
+    Kernel as Kernel,
+    total_variation_loss as total_variation_loss,
+    TotalVariationLoss as TotalVariationLoss,
+    frequency_reconstruction_loss as frequency_reconstruction_loss,
+    FrequencyReconstructionLoss as FrequencyReconstructionLoss,
+    edge_loss as edge_loss,
+    EdgeLoss as EdgeLoss,
+)
 from .utils import (
     check_vgg_params_exists as check_vgg_params_exists,
     load_vgg19_params as load_vgg19_params,
-    # get_loss_wrapper as get_loss_wrapper,
-    # compute_loss as compute_loss,
     Reduce as Reduces,
     LossWrapper as LossWrapper,
 )
 
 
 check_vgg_params_exists()
 del check_vgg_params_exists
```

### Comparing `flaxsr-0.0.5/flaxsr/losses/adversarial_losses.py` & `flaxsr-0.0.6/flaxsr/losses/adversarial_losses.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 from flaxsr.losses.utils import reduce_fn, Reduce, Loss
 from flaxsr._utils import register
 
 
 @partial(jax.jit, static_argnums=(2, 3,))
 def minmax_discriminator_loss(
-        true: jnp.ndarray, fake: jnp.ndarray, from_logits: bool = True, reduce: str | Reduce = 'mean',
+        fake: jnp.ndarray, true: jnp.ndarray, from_logits: bool = True, reduce: str | Reduce = 'mean',
         *args, **kwargs
 ):
     if from_logits:
         true_loss = -jax.nn.log_sigmoid(true)
         fake_loss = -jax.nn.log_sigmoid(-fake)
     else:
         true_loss = -jnp.log(true)
@@ -46,31 +46,31 @@
 
 @register('losses', 'minmax_discriminator')
 class MinmaxDiscriminatorLoss(Loss):
     def __init__(self, from_logits: bool = True, reduce: str | Reduce = 'mean'):
         super().__init__(reduce)
         self.from_logits = from_logits
 
-    def __call__(self, true: jnp.ndarray, fake: jnp.ndarray, *args, **kwargs):
-        return minmax_discriminator_loss(true, fake, self.from_logits, self.reduce)
+    def __call__(self, fake: jnp.ndarray, true: jnp.ndarray, *args, **kwargs):
+        return minmax_discriminator_loss(fake, true, self.from_logits, self.reduce)
 
 
 @register('losses', 'minmax_generator')
 class MinmaxGeneratorLoss(Loss):
     def __init__(self, from_logits: bool = True, reduce: str | Reduce = 'mean'):
         super().__init__(reduce)
         self.from_logits = from_logits
 
     def __call__(self, fake: jnp.ndarray, *args, **kwargs):
         return minmax_generator_loss(fake, self.from_logits, self.reduce)
 
 
 @partial(jax.jit, static_argnums=(2, 3,))
 def least_square_discriminator_loss(
-        true: jnp.ndarray, fake: jnp.ndarray, from_logits: bool = True, reduce: str | Reduce = 'mean',
+        fake: jnp.ndarray, true: jnp.ndarray, from_logits: bool = True, reduce: str | Reduce = 'mean',
         *args, **kwargs
 ):
     if from_logits:
         true = jax.nn.sigmoid(true)
         fake = jax.nn.sigmoid(fake)
 
     true_loss = .5 * jnp.square(true - 1.)
@@ -95,61 +95,61 @@
 
 @register('losses', 'least_square_discriminator')
 class LeastSquareDiscriminatorLoss(Loss):
     def __init__(self, from_logits: bool = True, reduce: str | Reduce = 'mean'):
         super().__init__(reduce)
         self.from_logits = from_logits
 
-    def __call__(self, true: jnp.ndarray, fake: jnp.ndarray, *args, **kwargs):
-        return least_square_discriminator_loss(true, fake, self.from_logits, self.reduce)
+    def __call__(self, fake: jnp.ndarray, true: jnp.ndarray, *args, **kwargs):
+        return least_square_discriminator_loss(fake, true, self.from_logits, self.reduce)
 
 
 @register('losses', 'least_square_generator')
 class LeastSquareGeneratorLoss(Loss):
     def __init__(self, from_logits: bool = True, reduce: str | Reduce = 'mean'):
         super().__init__(reduce)
         self.from_logits = from_logits
 
     def __call__(self, fake: jnp.ndarray, *args, **kwargs):
         return least_square_generator_loss(fake, self.from_logits, self.reduce)
 
 
 @partial(jax.jit, static_argnums=(2,))
 def relativistic_discriminator_loss(
-        true: jnp.ndarray, fake: jnp.ndarray, reduce: str | Reduce = 'mean',
+        fake: jnp.ndarray, true: jnp.ndarray, reduce: str | Reduce = 'mean',
         *args, **kwargs
 ):
     true_loss = -jax.nn.log_sigmoid(true - jnp.mean(fake))
     fake_loss = -jax.nn.log_sigmoid(-fake + jnp.mean(true))
 
     loss = true_loss + fake_loss
     return reduce_fn(loss, reduce)
 
 
 @partial(jax.jit, static_argnums=(2,))
 def relativistic_generator_loss(
-        true: jnp.ndarray, fake: jnp.ndarray, reduce: str | Reduce = 'mean',
+        fake: jnp.ndarray, true: jnp.ndarray, reduce: str | Reduce = 'mean',
         *args, **kwargs
 ):
     true_loss = -jax.nn.log_sigmoid(-true + jnp.mean(fake))
     fake_loss = -jax.nn.log_sigmoid(fake - jnp.mean(true))
 
     loss = true_loss + fake_loss
     return reduce_fn(loss, reduce)
 
 
 @register('losses', 'relativistic_discriminator')
 class RelativisticDiscriminatorLoss(Loss):
     def __init__(self, reduce: str | Reduce = 'mean'):
         super().__init__(reduce)
 
-    def __call__(self, true: jnp.ndarray, fake: jnp.ndarray, *args, **kwargs):
-        return relativistic_discriminator_loss(true, fake, self.reduce)
+    def __call__(self, fake: jnp.ndarray, true: jnp.ndarray, *args, **kwargs):
+        return relativistic_discriminator_loss(fake, true, self.reduce)
 
 
 @register('losses', 'relativistic_generator')
 class RelativisticGeneratorLoss(Loss):
     def __init__(self, reduce: str | Reduce = 'mean'):
         super().__init__(reduce)
 
-    def __call__(self, true: jnp.ndarray, fake: jnp.ndarray, *args, **kwargs):
-        return relativistic_generator_loss(true, fake, self.reduce)
+    def __call__(self, fake: jnp.ndarray, true: jnp.ndarray, *args, **kwargs):
+        return relativistic_generator_loss(fake, true, self.reduce)
```

### Comparing `flaxsr-0.0.5/flaxsr/losses/perceptual_losses.py` & `flaxsr-0.0.6/flaxsr/losses/perceptual_losses.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,22 +47,22 @@
             x = x  # for jax.jit
     outputs.append(x)
     return outputs
 
 
 @partial(jax.jit, static_argnums=(3, 5, 6,))
 def vgg_loss(
-        hr: jnp.ndarray, sr: jnp.ndarray, vgg_params: Pytree, feats_from: Sequence[int],
+        sr: jnp.ndarray, hr: jnp.ndarray, vgg_params: Pytree, feats_from: Sequence[int],
         mask: Optional[jnp.ndarray] = None, before_act: bool = False, reduce: str | Reduce = 'mean'
 ) -> jnp.ndarray:
     hr, sr = apply_mask(hr, sr, mask=mask)
     hr_feats = _get_feats_from_vgg19(hr, vgg_params, before_act)
     sr_feats = _get_feats_from_vgg19(sr, vgg_params, before_act)
 
-    loss = 0.
+    loss = jnp.zeros(())
     for i, (hr_feats, sr_feats) in enumerate(zip(hr_feats, sr_feats)):
         if i in feats_from:
             loss += jnp.mean((hr_feats - sr_feats) ** 2, axis=(1, 2, 3))
     return reduce_fn(loss, reduce)
 
 
 @register('losses', 'vgg')
@@ -71,16 +71,16 @@
             self, feats_from: Sequence[int], before_act: bool = False, reduce: str | Reduce = 'mean'
     ):
         super().__init__(reduce)
         self.feats_from = feats_from
         self.before_act = before_act
         self.vgg_params = load_vgg19_params()
 
-    def __call__(self, hr: jnp.ndarray, sr: jnp.ndarray, mask: Optional[jnp.ndarray] = None) -> jnp.ndarray:
-        return vgg_loss(hr, sr, self.vgg_params, self.feats_from, mask, self.before_act, self.reduce)
+    def __call__(self, sr: jnp.ndarray, hr: jnp.ndarray, mask: Optional[jnp.ndarray] = None) -> jnp.ndarray:
+        return vgg_loss(sr, hr, self.vgg_params, self.feats_from, mask, self.before_act, self.reduce)
 
 
 """
 Maybe Implement Style Loss in the future?
 1. _gram_matrix
 2. style_loss
 3. StyleLoss
```

### Comparing `flaxsr-0.0.5/flaxsr/losses/pixel_wise_losses.py` & `flaxsr-0.0.6/flaxsr/losses/pixel_wise_losses.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,59 +13,59 @@
 
 from flaxsr.losses.utils import reduce_fn, Reduce, Loss, apply_mask
 from flaxsr._utils import register
 
 
 @partial(jax.jit, static_argnums=(3,))
 def l1_loss(
-        hr: jnp.ndarray, sr: jnp.ndarray, mask: Optional[jnp.ndarray] = None, reduce: str | Reduce = 'mean'
+        sr: jnp.ndarray, hr: jnp.ndarray, mask: Optional[jnp.ndarray] = None, reduce: str | Reduce = 'mean'
 ) -> jnp.ndarray:
     hr, sr = apply_mask(hr, sr, mask=mask)
     loss = jnp.abs(hr - sr)
     return reduce_fn(loss, reduce)
 
 
 @register('losses', 'l1')
 class L1Loss(Loss):
     def __init__(self, reduce: str | Reduce = 'mean'):
         super().__init__(reduce=reduce)
 
-    def __call__(self, hr: jnp.ndarray, sr: jnp.ndarray, mask: Optional[jnp.ndarray] = None) -> jnp.ndarray:
-        return l1_loss(hr, sr, mask=mask, reduce=self.reduce)
+    def __call__(self, sr: jnp.ndarray, hr: jnp.ndarray, mask: Optional[jnp.ndarray] = None) -> jnp.ndarray:
+        return l1_loss(sr, hr, mask=mask, reduce=self.reduce)
 
 
 @partial(jax.jit, static_argnums=(3,))
 def l2_loss(
-        hr: jnp.ndarray, sr: jnp.ndarray, mask: Optional[jnp.ndarray] = None, reduce: str | Reduce = 'mean'
+        sr: jnp.ndarray, hr: jnp.ndarray, mask: Optional[jnp.ndarray] = None, reduce: str | Reduce = 'mean'
 ) -> jnp.ndarray:
     hr, sr = apply_mask(hr, sr, mask=mask)
     loss = jnp.square(hr - sr)
     return reduce_fn(loss, reduce)
 
 
 @register('losses', 'l2')
 class L2Loss(Loss):
     def __init__(self, reduce: str | Reduce = 'mean'):
         super().__init__(reduce)
 
-    def __call__(self, hr: jnp.ndarray, sr: jnp.ndarray, mask: Optional[jnp.ndarray] = None) -> jnp.ndarray:
-        return l2_loss(hr, sr, mask=mask, reduce=self.reduce)
+    def __call__(self, sr: jnp.ndarray, hr: jnp.ndarray, mask: Optional[jnp.ndarray] = None) -> jnp.ndarray:
+        return l2_loss(sr, hr, mask=mask, reduce=self.reduce)
 
 
 @partial(jax.jit, static_argnums=(4,))
 def charbonnier_loss(
-        hr: jnp.ndarray, sr: jnp.ndarray, eps: float = 1e-3, mask: Optional[jnp.ndarray] = None,
+        sr: jnp.ndarray, hr: jnp.ndarray,  eps: float = 1e-3, mask: Optional[jnp.ndarray] = None,
         reduce: str | Reduce = 'mean'
 ) -> jnp.ndarray:
     hr, sr = apply_mask(hr, sr, mask=mask)
     loss = jnp.sqrt(jnp.square(hr - sr) + eps ** 2)
     return reduce_fn(loss, reduce)
 
 
 @register('losses', 'charbonnier')
 class CharbonnierLoss(Loss):
     def __init__(self, eps: float = 1e-3, reduce: str | Reduce = 'mean'):
         super().__init__(reduce)
         self.eps = eps
 
-    def __call__(self, hr: jnp.ndarray, sr: jnp.ndarray, mask: Optional[jnp.ndarray] = None) -> jnp.ndarray:
-        return charbonnier_loss(hr, sr, self.eps, mask, self.reduce)
+    def __call__(self, sr: jnp.ndarray, hr: jnp.ndarray, mask: Optional[jnp.ndarray] = None) -> jnp.ndarray:
+        return charbonnier_loss(sr, hr, self.eps, mask, self.reduce)
```

### Comparing `flaxsr-0.0.5/flaxsr/losses/utils.py` & `flaxsr-0.0.6/flaxsr/losses/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -38,23 +38,28 @@
         pass
 
 
 def reduce_fn(loss, reduce: str | Reduce) -> jnp.ndarray:
     if isinstance(reduce, str):
         reduce = Reduce(reduce)
 
+    reduce_axis = tuple(range(1, len(loss.shape)))
+
     if reduce == Reduce.SUM:
-        return jnp.sum(loss)
+        stat = jnp.sum(loss, axis=reduce_axis)
     elif reduce == Reduce.MEAN:
-        return jnp.mean(loss)
+        stat = jnp.mean(loss, axis=reduce_axis)
     elif reduce == Reduce.NONE:
         return loss
     else:
         raise ValueError(f"Unknown reduce type {reduce}")
 
+    stat = jnp.mean(stat)
+    return stat
+
 
 def apply_mask(*args, mask: Optional[jnp.ndarray]) -> tuple[jnp.ndarray, ...]:
     if mask is None:
         return args
     return tuple(arg * mask for arg in args)
 
 
@@ -98,14 +103,14 @@
         assert all(True if reduce in ['none', Reduce.NONE] else False for reduce in reduces) or \
                all(True if reduce not in ['none', Reduce.NONE] else False for reduce in reduces), \
             f'Cannot use None with others(Sum, Mean), got {reduces}'
 
         self.losses = losses
         self.weights = weights
 
-    def __call__(self, hr: jnp.ndarray, sr: jnp.ndarray, mask: Optional[jnp.ndarray] = None) -> jnp.ndarray:
+    def __call__(self, sr: jnp.ndarray, hr: jnp.ndarray, mask: Optional[jnp.ndarray] = None) -> jnp.ndarray:
         loss = jnp.zeros(())
 
         for loss_fn, weight in zip(self.losses, self.weights):
-            loss += weight * loss_fn(hr, sr, mask)
+            loss += weight * loss_fn(sr, hr, mask)
 
         return loss
```

### Comparing `flaxsr-0.0.5/flaxsr/models/edsr.py` & `flaxsr-0.0.6/flaxsr/models/edsr.py`

 * *Files identical despite different names*

### Comparing `flaxsr-0.0.5/flaxsr/models/espcn.py` & `flaxsr-0.0.6/flaxsr/models/espcn.py`

 * *Files identical despite different names*

### Comparing `flaxsr-0.0.5/flaxsr/models/fsrcnn.py` & `flaxsr-0.0.6/flaxsr/models/fsrcnn.py`

 * *Files identical despite different names*

### Comparing `flaxsr-0.0.5/flaxsr/models/nafssr.py` & `flaxsr-0.0.6/flaxsr/models/nafssr.py`

 * *Files identical despite different names*

### Comparing `flaxsr-0.0.5/flaxsr/models/ncnet.py` & `flaxsr-0.0.6/flaxsr/models/ncnet.py`

 * *Files identical despite different names*

### Comparing `flaxsr-0.0.5/flaxsr/models/srcnn.py` & `flaxsr-0.0.6/flaxsr/models/srcnn.py`

 * *Files identical despite different names*

### Comparing `flaxsr-0.0.5/flaxsr/models/srgan.py` & `flaxsr-0.0.6/flaxsr/models/srgan.py`

 * *Files identical despite different names*

### Comparing `flaxsr-0.0.5/flaxsr/models/vdsr.py` & `flaxsr-0.0.6/flaxsr/models/vdsr.py`

 * *Files identical despite different names*

### Comparing `flaxsr-0.0.5/flaxsr/training/train_step.py` & `flaxsr-0.0.6/flaxsr/training/train_step.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     if len(batch) == 2:
         lr, hr = batch
     else:
         lr, hr, mask = batch
 
     def loss_fn(params):
         _sr = state.apply_fn(params, lr)
-        _loss = state.losses(hr, _sr, mask if len(batch) == 3 else None)
+        _loss = state.losses(_sr, hr, mask if len(batch) == 3 else None)
         return _loss, _sr
 
     grad_fn = jax.value_and_grad(loss_fn, has_aux=True)
     (loss, sr), grad = grad_fn(state.params)
     state = state.apply_gradients(grads=grad)
     return state, loss
```

### Comparing `flaxsr-0.0.5/flaxsr.egg-info/SOURCES.txt` & `flaxsr-0.0.6/flaxsr.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 flaxsr/layers/__init__.py
 flaxsr/layers/stochastic.py
 flaxsr/layers/upscale.py
 flaxsr/losses/__init__.py
 flaxsr/losses/adversarial_losses.py
 flaxsr/losses/perceptual_losses.py
 flaxsr/losses/pixel_wise_losses.py
+flaxsr/losses/regularization_losses.py
 flaxsr/losses/utils.py
 flaxsr/models/__init__.py
 flaxsr/models/edsr.py
 flaxsr/models/espcn.py
 flaxsr/models/fsrcnn.py
 flaxsr/models/nafssr.py
 flaxsr/models/ncnet.py
```

### Comparing `flaxsr-0.0.5/setup.py` & `flaxsr-0.0.6/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import setuptools
 
 
 setuptools.setup(
     name="flaxsr",
-    version="0.0.5",
+    version="0.0.6",
     author="dslisleedh",
     author_email="dslisleedh@gmail.com",
-    description="Super Resolution models with Jax/Flax",
+    description="Super Resolution tools with Jax/Flax",
     long_description=open('README.md', 'rt').read(),
     long_description_content_type="text/markdown",
     url="https://github.com/dslisleedh/FlaxSR",
     project_urls={
         "Bug Tracker": "https://github.com/dslisleedh/FlaxSR/issues",
     },
     classifiers=[
```

