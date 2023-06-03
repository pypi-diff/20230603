# Comparing `tmp/jaxrenderer-0.1.3.tar.gz` & `tmp/jaxrenderer-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jaxrenderer-0.1.3.tar", max compression
+gzip compressed data, was "jaxrenderer-0.2.0.tar", max compression
```

## Comparing `jaxrenderer-0.1.3.tar` & `jaxrenderer-0.2.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0    11367 2023-06-02 15:14:13.067642 jaxrenderer-0.1.3/LICENSE
--rw-r--r--   0        0        0     1866 2023-06-02 15:14:13.067642 jaxrenderer-0.1.3/README.md
--rw-r--r--   0        0        0     4148 2023-06-02 15:14:13.067642 jaxrenderer-0.1.3/changelog.md
--rw-r--r--   0        0        0     1540 2023-06-02 15:14:13.067642 jaxrenderer-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     4851 2023-06-02 15:14:13.067642 jaxrenderer-0.1.3/renderer/README.md
--rw-r--r--   0        0        0      459 2023-06-02 15:14:13.067642 jaxrenderer-0.1.3/renderer/__init__.py
--rw-r--r--   0        0        0    33725 2023-06-02 15:14:13.067642 jaxrenderer-0.1.3/renderer/geometry.py
--rw-r--r--   0        0        0    14815 2023-06-02 15:14:13.067642 jaxrenderer-0.1.3/renderer/model.py
--rw-r--r--   0        0        0    11913 2023-06-02 15:14:13.067642 jaxrenderer-0.1.3/renderer/pipeline.py
--rw-r--r--   0        0        0    13883 2023-06-02 15:14:13.067642 jaxrenderer-0.1.3/renderer/renderer.py
--rw-r--r--   0        0        0     9726 2023-06-02 15:14:13.067642 jaxrenderer-0.1.3/renderer/scene.py
--rw-r--r--   0        0        0    10102 2023-06-02 15:14:13.071642 jaxrenderer-0.1.3/renderer/shader.py
--rw-r--r--   0        0        0     4600 2023-06-02 15:14:13.071642 jaxrenderer-0.1.3/renderer/shaders/README.md
--rw-r--r--   0        0        0     1256 2023-06-02 15:14:13.071642 jaxrenderer-0.1.3/renderer/shaders/depth.py
--rw-r--r--   0        0        0     3252 2023-06-02 15:14:13.071642 jaxrenderer-0.1.3/renderer/shaders/gouraud.py
--rw-r--r--   0        0        0     4804 2023-06-02 15:14:13.071642 jaxrenderer-0.1.3/renderer/shaders/gouraud_texture.py
--rw-r--r--   0        0        0     5079 2023-06-02 15:14:13.071642 jaxrenderer-0.1.3/renderer/shaders/phong.py
--rw-r--r--   0        0        0     9571 2023-06-02 15:14:13.071642 jaxrenderer-0.1.3/renderer/shaders/phong_darboux.py
--rw-r--r--   0        0        0     7926 2023-06-02 15:14:13.071642 jaxrenderer-0.1.3/renderer/shaders/phong_reflection.py
--rw-r--r--   0        0        0     9650 2023-06-02 15:14:13.071642 jaxrenderer-0.1.3/renderer/shaders/phong_reflection_shadow.py
--rw-r--r--   0        0        0     4166 2023-06-02 15:14:13.071642 jaxrenderer-0.1.3/renderer/shadow.py
--rw-r--r--   0        0        0    71549 2023-06-02 15:14:13.071642 jaxrenderer-0.1.3/renderer/shapes/capsule.py
--rw-r--r--   0        0        0     3574 2023-06-02 15:14:13.071642 jaxrenderer-0.1.3/renderer/shapes/cube.py
--rw-r--r--   0        0        0     3270 2023-06-02 15:14:13.071642 jaxrenderer-0.1.3/renderer/types.py
--rw-r--r--   0        0        0     3074 2023-06-02 15:14:13.071642 jaxrenderer-0.1.3/renderer/utils.py
--rw-r--r--   0        0        0      833 2023-06-02 15:14:13.071642 jaxrenderer-0.1.3/renderer/value_checker.py
--rw-r--r--   0        0        0     3320 1970-01-01 00:00:00.000000 jaxrenderer-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0    11367 2023-06-03 14:29:52.493212 jaxrenderer-0.2.0/LICENSE
+-rw-r--r--   0        0        0     2312 2023-06-03 14:29:52.493212 jaxrenderer-0.2.0/README.md
+-rw-r--r--   0        0        0     4530 2023-06-03 14:29:52.493212 jaxrenderer-0.2.0/changelog.md
+-rw-r--r--   0        0        0     1540 2023-06-03 14:29:52.493212 jaxrenderer-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     4851 2023-06-03 14:29:52.493212 jaxrenderer-0.2.0/renderer/README.md
+-rw-r--r--   0        0        0      459 2023-06-03 14:29:52.493212 jaxrenderer-0.2.0/renderer/__init__.py
+-rw-r--r--   0        0        0    33725 2023-06-03 14:29:52.493212 jaxrenderer-0.2.0/renderer/geometry.py
+-rw-r--r--   0        0        0    14815 2023-06-03 14:29:52.493212 jaxrenderer-0.2.0/renderer/model.py
+-rw-r--r--   0        0        0    13911 2023-06-03 14:29:52.497212 jaxrenderer-0.2.0/renderer/pipeline.py
+-rw-r--r--   0        0        0    13883 2023-06-03 14:29:52.497212 jaxrenderer-0.2.0/renderer/renderer.py
+-rw-r--r--   0        0        0     9726 2023-06-03 14:29:52.497212 jaxrenderer-0.2.0/renderer/scene.py
+-rw-r--r--   0        0        0    10102 2023-06-03 14:29:52.497212 jaxrenderer-0.2.0/renderer/shader.py
+-rw-r--r--   0        0        0     4600 2023-06-03 14:29:52.497212 jaxrenderer-0.2.0/renderer/shaders/README.md
+-rw-r--r--   0        0        0     1256 2023-06-03 14:29:52.497212 jaxrenderer-0.2.0/renderer/shaders/depth.py
+-rw-r--r--   0        0        0     3252 2023-06-03 14:29:52.497212 jaxrenderer-0.2.0/renderer/shaders/gouraud.py
+-rw-r--r--   0        0        0     4804 2023-06-03 14:29:52.497212 jaxrenderer-0.2.0/renderer/shaders/gouraud_texture.py
+-rw-r--r--   0        0        0     5079 2023-06-03 14:29:52.497212 jaxrenderer-0.2.0/renderer/shaders/phong.py
+-rw-r--r--   0        0        0     9571 2023-06-03 14:29:52.497212 jaxrenderer-0.2.0/renderer/shaders/phong_darboux.py
+-rw-r--r--   0        0        0     7926 2023-06-03 14:29:52.497212 jaxrenderer-0.2.0/renderer/shaders/phong_reflection.py
+-rw-r--r--   0        0        0     9650 2023-06-03 14:29:52.497212 jaxrenderer-0.2.0/renderer/shaders/phong_reflection_shadow.py
+-rw-r--r--   0        0        0     4166 2023-06-03 14:29:52.497212 jaxrenderer-0.2.0/renderer/shadow.py
+-rw-r--r--   0        0        0    71549 2023-06-03 14:29:52.497212 jaxrenderer-0.2.0/renderer/shapes/capsule.py
+-rw-r--r--   0        0        0     3574 2023-06-03 14:29:52.497212 jaxrenderer-0.2.0/renderer/shapes/cube.py
+-rw-r--r--   0        0        0     3270 2023-06-03 14:29:52.497212 jaxrenderer-0.2.0/renderer/types.py
+-rw-r--r--   0        0        0     3074 2023-06-03 14:29:52.497212 jaxrenderer-0.2.0/renderer/utils.py
+-rw-r--r--   0        0        0      833 2023-06-03 14:29:52.497212 jaxrenderer-0.2.0/renderer/value_checker.py
+-rw-r--r--   0        0        0     3766 1970-01-01 00:00:00.000000 jaxrenderer-0.2.0/PKG-INFO
```

### Comparing `jaxrenderer-0.1.3/LICENSE` & `jaxrenderer-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `jaxrenderer-0.1.3/README.md` & `jaxrenderer-0.2.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -4,17 +4,20 @@
 
 - Native JAX implementation, supports `jit`, `vmap`, etc.
 - Lighting is computed in main camera's eye space; while in PyTinyrenderer it is computed in world space.
 - Texture specification is different: in PyTinyrenderer, the texture is specified in a flattened array, while in JAX Renderer, the texture is specified in a shape of (width, height, colour channels). A simple way to transform old specification to new specification is to use the convenient method `build_texture_from_PyTinyrenderer`.
 - Rendering pipeline is different. PyTinyrenderer renders one object at a time, and share zbuffer and framebuffer across one pass. This renderer first merges all objects into one big mesh in world space, then process all vertices together, then interpolates and rasterise and render. For fragment shading, this is done by sweeping each row in a for loop, and batch compute all pixels together. For computing a pixel, all fragments for that pixels are batch compute together, then mixed. This is more memory efficient and allows `vmap` batching as far as possible.
 - Shadowing within the same object / mesh is allowed. This is not possible in PyTinyrenderer, as it deliberately checks if the shadow comes from the same object; if so, it will not consider to draw a shadow there.
 - Quaternion (for specifying rotation/orientation) is in the form of `(w, x, y, z)` instead of `(x, y, z, w)` in PyTinyrenderer. This is for consistency with `BRAX`.
+- No clipping is performed. To ensure correct rendering of objects with vertices at or behind camera plane, homogeneous interpolation (Olano and Greer, 1997)[^1] is used to avoid the need of homogeneous division.
 - Fix bugs
   - Specular lighting was wrong, where it forgets to reverse the light direction vector.
 
+[^1]: Marc Olano and Trey Greer. 1997. Triangle Scan Conversion Using 2D Homogeneous Coordinates. In _Proceedings of the ACM SIGGRAPH/EUROGRAPHICS Workshop on Graphics Hardware (HWWS ’97)_. ACM, New York, NY, USA, 89–95.
+
 ## Roadmap
 
-- [ ] Correctly implement a proper clipping algorithm
 - [ ] Support double-sided objects
 - [ ] Profile and accelerate implementation
 - [ ] Differentiable rendering
 - [ ] Build a ray tracer as well
+- [ ] <s>Correctly implement a proper clipping algorithm</s>
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `jaxrenderer-0.1.3/changelog.md` & `jaxrenderer-0.2.0/changelog.md`

 * *Files 5% similar despite different names*

```diff
@@ -35,7 +35,12 @@
 5. Downgrade minimum Python version to `3.9`, `numpy` version to `1.22.0`, `jax` and `jaxlib` version to `0.4.4`.
 
 ## 0.1.3
 
 1. Correctly force convert `LightParameters` to JAX arrays in `Renderer.get_camera_image` to avoid downstream errors.
 2. Fix `geometry.py::transform_matrix_from_rotation`. Also, change the order of quaternion to `(w, x, y, z)` instead of `(x, y, z, w)` for consistency.
 3. Force convert `ShadowParameters` to JAX arrays in `Renderer.get_camera_image` to avoid downstream errors.
+
+## 0.2.0
+
+1. Instead of clipping (planned to be implemented), now the rasteriser interpolates in homogeneous space directly. `Shader.interpolate` will not receive valid `barycentric_screen` values for now. Setting `Interpolation.SMOOTH` and `Interpolation.NOPERSPECTIVE` will result in same results, perspective-correct interpolations.
+2. Reorganise example files and rename them.
```

### Comparing `jaxrenderer-0.1.3/pyproject.toml` & `jaxrenderer-0.2.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "jaxrenderer"
-version = "0.1.3"
+version = "0.2.0"
 description = "Jax implementation of rasterizer renderer."
 authors = ["Joey Teng <joey.teng.dev@gmail.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 homepage = "https://github.com/JoeyTeng/jaxrenderer"
 repository = "https://github.com/JoeyTeng/jaxrenderer"
 classifiers = [
```

### Comparing `jaxrenderer-0.1.3/renderer/README.md` & `jaxrenderer-0.2.0/renderer/README.md`

 * *Files identical despite different names*

### Comparing `jaxrenderer-0.1.3/renderer/geometry.py` & `jaxrenderer-0.2.0/renderer/geometry.py`

 * *Files identical despite different names*

### Comparing `jaxrenderer-0.1.3/renderer/model.py` & `jaxrenderer-0.2.0/renderer/model.py`

 * *Files identical despite different names*

### Comparing `jaxrenderer-0.1.3/renderer/pipeline.py` & `jaxrenderer-0.2.0/renderer/pipeline.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,58 +1,98 @@
 from functools import partial
-from typing import Any, NamedTuple, TypeVar, Union
+from typing import Any, NamedTuple, TypeVar
 
 import jax
 import jax.lax as lax
 import jax.numpy as jnp
 from jax import lax
 from jax.tree_util import tree_map
 from jaxtyping import Array, Bool, Float, Integer, Num, jaxtyped
 
-from .geometry import (Camera, Interpolation, barycentric, interpolate,
-                       normalise_homogeneous)
+from .geometry import Camera, Interpolation, Viewport, interpolate
 from .shader import (ID, MixedExtraT, MixerOutput, PerFragment, PerVertex,
                      Shader, ShaderExtraInputT, VaryingT)
-from .types import (FALSE_ARRAY, Buffers, FaceIndices, Triangle, Triangle2Df,
-                    Vec2f, Vec2i, Vec3f, Vec4f)
+from .types import (FALSE_ARRAY, Buffers, FaceIndices, Triangle, Vec2f, Vec2i,
+                    Vec3f, Vec4f)
 
 jax.config.update('jax_array', True)
 
 
-class PerVertexInScreen(NamedTuple):
-    """Built-in output from Vertex Shader after Viewport transformation.
-
-    gl_Position is in screen-space.
-    """
-    gl_Position: Vec4f
-    # gl_PointSize is meaningful only when rendering point primitives.
-    # not supported for now
-    # gl_PointSize: Float[Array, ""]
-
-
 class PerPrimitive(NamedTuple):
     """Input for each primitive, using outputs from Vertex Shader.
 
-    gl_Position is in screen-space, normalised homogeneous coordinate
+    gl_Position is in clip-space, not normalised.
     """
     gl_Position: Triangle
     # gl_PointSize is meaningful only when rendering point primitives.
     # not supported for now
     # gl_PointSize: Float[Array, "primitives"]
+    keep: Bool[Array, ""]
+    """Whether to keep this primitive for rasterisation.
+        !!Never keep a primitive with a zero determinant.
+    """
+    determinant: Float[Array, ""]
+    """determinant of the matrix with [x, y, w] of the three vertices in clip
+        space, in a shape of
+
+        [[x0, y0, w0],
+         [x1, y1, w1],
+         [x2, y2, w2]].
+
+        When determinant is 0, the triangle will not be rendered for now.
+    """
+    matrix_inv: Float[Array, "3 3"]
+    """inverse of the matrix described above (of [x, y, w])."""
+
+    @classmethod
+    @jaxtyped
+    @partial(jax.jit, static_argnames=("cls", ))
+    def create(cls, per_vertex: PerVertex) -> "PerPrimitive":
+        """per_vertex is batched with size 3 (3 vertices per triangle)
+            in clip-space, not normalised.
+        """
+        clip: Triangle = per_vertex.gl_Position
+        assert isinstance(clip, Triangle)
+        # matrix with x, y, w
+        matrix: Float[Array, "3 3"] = clip[:, jnp.array((0, 1, 3))]
+        # If == 0, the matrix inverse does not exist, should use another
+        # interpolation method. Early exit for now.
+        # `jnp.linalg.det` has built-in 3x3 det optimisation
+        determinant: Float[Array, ""] = jnp.linalg.det(matrix)
+        assert isinstance(determinant, Float[Array, ""])
+
+        # an arbitrary number for numerical stability
+        keep: Bool[Array, ""] = lax.abs(determinant) > 1e-6
+
+        mat_inv: Float[Array, "3 3"] = lax.cond(
+            # an arbitrary number for numerical stability
+            keep,
+            # may replace with custom implementation for higher precision
+            lambda: jnp.linalg.inv(matrix),
+            lambda: jnp.zeros((3, 3)),
+        )
+        assert isinstance(mat_inv, Float[Array, "3 3"])
+
+        return cls(
+            gl_Position=clip,
+            keep=keep,
+            determinant=determinant,
+            matrix_inv=mat_inv,
+        )
 
 
 @jaxtyped
 @partial(jax.jit, static_argnames=("shader", ), donate_argnums=(1, ))
 def _postprocessing(
-    shader: Union[Shader[ShaderExtraInputT, VaryingT, MixedExtraT],
-                  type[Shader[ShaderExtraInputT, VaryingT, MixedExtraT]]],
+    shader: type[Shader[ShaderExtraInputT, VaryingT, MixedExtraT]],
     buffers: Buffers,
     per_primitive: tuple[Any, ...],  # Batch PerPrimitive
     varyings: VaryingT,
     extra: ShaderExtraInputT,
+    viewport: Viewport,
 ) -> Buffers:
     with jax.ensure_compile_time_eval():
         # loop along first axis, for memory efficiency
         # TODO: benchmark if this is actually faster
         loop_size: int = int(buffers[0].shape[0])
         # vmap batch along second axis
         batch_size: int = int(buffers[0].shape[1])
@@ -64,66 +104,86 @@
         assert isinstance(coord, Vec2i), f"expected Vec2i, got {coord}"
 
         @jaxtyped
         def _per_primitive_process(
             primitive: PerPrimitive,
             varying_per_primitive: VaryingT,
         ) -> tuple[PerFragment, VaryingT]:
-            screen: Triangle = primitive.gl_Position
-
-            # 2d screen coordinates
-            screen2d: Triangle2Df = screen[:, :2]
-            assert isinstance(screen2d, Triangle2Df)
-
-            # PROCESS: Rasterisation (Interpolate)
-            # barycentric coordinates
-            bc_screen: Vec3f = barycentric(screen2d, coord)
-            assert isinstance(bc_screen, Vec3f)
-
-            def _when_keep_triangle() -> tuple[PerFragment, VaryingT]:
-                # weight barycentric coordinates by 1/w to obtain
-                # perspective-coorected barycentric coordinates
-                bc_clip: Vec3f = bc_screen * screen[:, 3]
+            # PROCESS: Interpolation
 
-                # normalise barycentric coordinates so that it sums to 1.
-                bc_clip = bc_clip / bc_clip.sum()
+            # For early exit when not keep primitive / determinant is 0
+            def _when_keep_primitive() -> tuple[Vec3f, Float[Array, ""]]:
+                """Returns clip_coef, w_reciprocal."""
+                # x/w, y/w, with x, y, w in clip space.
+                xy: Float[Array, "2"] = (
+                    (coord - viewport[:2, 3]) /
+                    viewport[jnp.arange(2), jnp.arange(2)])
+                xy1_ndc: Float[Array, "3"] = jnp.array((xy[0], xy[1], 1))
+
+                # As the interpolation formula is `xy1_ndc @ (mat_inv @ values)`
+                # we can utilise associativity to generate a set of fixed Vec3f
+                # coefficient for interpolation.
+                # Noticed that this is also the "edge function" values, with
+                # a pseudo-parameter that is zero at the two vertices on the
+                # edge and one at the opposite vertex, as described
+                # in [Olano and Greer, 1997].
+                clip_coef: Vec3f = jnp.dot(xy1_ndc, primitive.matrix_inv)
+                assert isinstance(clip_coef, Vec3f)
+                # 1/w, w in clip space.
+                w_reciprocal: Float[Array, ""] = clip_coef.sum()
+                assert isinstance(w_reciprocal, Float[Array, ""])
+
+                return clip_coef, w_reciprocal
+
+            # END OF `_when_keep_primitive`
+
+            # Prepare for interpolation parameters
+            # clip_coef here interpolates to 1/w * target value
+            clip_coef, w_reciprocal = lax.cond(
+                # an arbitrary number for numerical stability
+                primitive.keep,
+                _when_keep_primitive,
+                lambda: (lax.full((3, ), -1.), jnp.zeros(())),
+            )
 
+            def _when_in_triangle() -> tuple[PerFragment, VaryingT]:
                 # Prepare inputs for fragment shader
-                # no need to "normalise" as barycentric coordinates here
-                # ensures it sums to 1, thus result is normalised when inputs
-                # are.
-                # Mode: NOPERSPECTIVE: since inverse of the depth is linear,
-                # the correct way to interpolate it is just to interpolate
-                # under screen space using bc_screen,
-                # or using `NONPERSPECTVIE` mode.
-                gl_FragCoord: Vec4f = interpolate(
-                    screen,
-                    bc_screen,
-                    bc_clip,
-                    mode=Interpolation.NOPERSPECTIVE,
+                z: Float[Array, ""] = interpolate(
+                    values=primitive.gl_Position[:, 2],
+                    barycentric_screen=clip_coef,
+                    barycentric_clip=clip_coef,
+                    mode=Interpolation.SMOOTH,
                 )
-                gl_FragCoord.at[:2].set(coord)
+                # viewport transform for z, from clip space to window space
+                z = z * viewport[2, 2] + viewport[2, 3]
+                gl_FragCoord: Vec4f = jnp.array((
+                    coord[0],
+                    coord[1],
+                    z,
+                    w_reciprocal,
+                ))
                 assert isinstance(gl_FragCoord, Vec4f)
 
                 # Ref: https://registry.khronos.org/OpenGL-Refpages/gl4/html/gl_FrontFacing.xhtml
-                gl_FrontFacing: Bool[Array, ""] = jnp.cross(
-                    screen[1, :3] - screen[0, :3],
-                    screen[2, :3] - screen[0, :3],
-                )[-1] > 0
+                gl_FrontFacing: Bool[Array, ""] = primitive.determinant > 0
                 assert isinstance(gl_FrontFacing, Bool[Array, ""])
 
                 gl_PointCoord: Vec2f
                 with jax.ensure_compile_time_eval():
                     # TODO: implement Point primitive properly.
                     gl_PointCoord = lax.full((2, ), 0)
 
+                # this interpolates to target value u, not u/w
+                true_clip_coef: Vec3f = clip_coef / w_reciprocal
+                assert isinstance(true_clip_coef, Vec3f)
+
                 varying: VaryingT = shader.interpolate(
-                    varying_per_primitive,
-                    bc_screen,
-                    bc_clip,
+                    values=varying_per_primitive,
+                    barycentric_screen=true_clip_coef,
+                    barycentric_clip=true_clip_coef,
                 )
                 assert isinstance(varying, tuple)
 
                 # PROCESS: Fragment Processing
                 per_frag: PerFragment
                 extra_fragment_output: VaryingT
                 per_frag, extra_fragment_output = shader.fragment(
@@ -142,24 +202,24 @@
                     lambda: per_frag._replace(gl_FragDepth=gl_FragCoord[2]),
                     lambda: per_frag,
                 )
                 assert isinstance(per_frag, PerFragment)
 
                 return per_frag, extra_fragment_output
 
-            # END OF `_when_keep_triangle`
+            # END OF `_when_in_triangle`
 
-            in_triangle: Bool[Array, ""] = (bc_screen >= 0).all()
+            in_triangle: Bool[Array, ""] = (clip_coef >= 0).all()
             assert isinstance(in_triangle, Bool[Array, ""])
 
             built_in: PerFragment
             attachments: VaryingT
             built_in, attachments = lax.cond(
-                in_triangle,
-                _when_keep_triangle,
+                jnp.logical_and(primitive.keep, in_triangle),
+                _when_in_triangle,
                 # discard out-of-triangle values
                 lambda: (
                     PerFragment(keeps=FALSE_ARRAY),
                     # dummy values
                     tree_map(lambda field: field[0], varying_per_primitive),
                 ),
             )
@@ -269,16 +329,15 @@
     return buffers
 
 
 @jaxtyped
 @partial(jax.jit, static_argnames=("shader", ), donate_argnums=(2, ))
 def render(
     camera: Camera,
-    shader: Union[Shader[ShaderExtraInputT, VaryingT, MixedExtraT],
-                  type[Shader[ShaderExtraInputT, VaryingT, MixedExtraT]]],
+    shader: type[Shader[ShaderExtraInputT, VaryingT, MixedExtraT]],
     buffers: Buffers,
     face_indices: FaceIndices,
     extra: ShaderExtraInputT,
 ) -> Buffers:
     vertices_count: int
     gl_InstanceID: ID
     with jax.ensure_compile_time_eval():
@@ -287,52 +346,42 @@
         assert isinstance(vertices_count, int)
         assert isinstance(gl_InstanceID, ID)
 
     @jaxtyped
     @jax.jit
     def vertex_processing(
             gl_VertexID: Integer[Array, ""],  #
-    ) -> tuple[PerVertexInScreen, VaryingT]:
+    ) -> tuple[PerVertex, VaryingT]:
         """Process one vertex into screen space, and keep varying values."""
         per_vertex: PerVertex
         varying: VaryingT
         per_vertex, varying = shader.vertex(
             gl_VertexID,
             gl_InstanceID,
             camera,
             extra,
         )
         assert isinstance(per_vertex, PerVertex)
         assert isinstance(varying, tuple)
 
-        # TODO: add clipping in clip space.
-
-        # NDC, normalised device coordinate
-        # Ref: OpenGL Spec 4.6 (Core Profile), Section 15.2.2
-        w: Float[Array, ""] = per_vertex.gl_Position[3]
-        ndc: Vec4f = normalise_homogeneous(per_vertex.gl_Position)
-        assert isinstance(ndc, Vec4f)
-
-        # already normalised; result is still normalised
-        # Ref: OpenGL Spec 4.6 (Core Profile), Section 15.2.2
-        screen: Vec4f = (camera.viewport @ ndc).at[3].divide(w)
-        assert isinstance(screen, Vec4f)
-
-        return PerVertexInScreen(gl_Position=screen), varying
+        return per_vertex, varying
 
     # PROCESS: Vertex Processing
     per_vertices, varyings = jax.vmap(vertex_processing)(
         lax.iota(int, vertices_count),  # gl_VertexID
     )
 
     # everything after vertex processing, will directly update buffers
     buffers = _postprocessing(
         shader=shader,
         buffers=buffers,
-        per_primitive=tree_map(lambda field: field[face_indices],
-                               per_vertices),
+        per_primitive=jax.vmap(PerPrimitive.create)(tree_map(
+            lambda field: field[face_indices],
+            per_vertices,
+        )),
         varyings=tree_map(lambda field: field[face_indices], varyings),
         extra=extra,
+        viewport=camera.viewport,
     )
     assert isinstance(buffers, Buffers)
 
     return buffers
```

### Comparing `jaxrenderer-0.1.3/renderer/renderer.py` & `jaxrenderer-0.2.0/renderer/renderer.py`

 * *Files identical despite different names*

### Comparing `jaxrenderer-0.1.3/renderer/scene.py` & `jaxrenderer-0.2.0/renderer/scene.py`

 * *Files identical despite different names*

### Comparing `jaxrenderer-0.1.3/renderer/shader.py` & `jaxrenderer-0.2.0/renderer/shader.py`

 * *Files identical despite different names*

### Comparing `jaxrenderer-0.1.3/renderer/shaders/README.md` & `jaxrenderer-0.2.0/renderer/shaders/README.md`

 * *Files identical despite different names*

### Comparing `jaxrenderer-0.1.3/renderer/shaders/depth.py` & `jaxrenderer-0.2.0/renderer/shaders/depth.py`

 * *Files identical despite different names*

### Comparing `jaxrenderer-0.1.3/renderer/shaders/gouraud.py` & `jaxrenderer-0.2.0/renderer/shaders/gouraud.py`

 * *Files identical despite different names*

### Comparing `jaxrenderer-0.1.3/renderer/shaders/gouraud_texture.py` & `jaxrenderer-0.2.0/renderer/shaders/gouraud_texture.py`

 * *Files identical despite different names*

### Comparing `jaxrenderer-0.1.3/renderer/shaders/phong.py` & `jaxrenderer-0.2.0/renderer/shaders/phong.py`

 * *Files identical despite different names*

### Comparing `jaxrenderer-0.1.3/renderer/shaders/phong_darboux.py` & `jaxrenderer-0.2.0/renderer/shaders/phong_darboux.py`

 * *Files identical despite different names*

### Comparing `jaxrenderer-0.1.3/renderer/shaders/phong_reflection.py` & `jaxrenderer-0.2.0/renderer/shaders/phong_reflection.py`

 * *Files identical despite different names*

### Comparing `jaxrenderer-0.1.3/renderer/shaders/phong_reflection_shadow.py` & `jaxrenderer-0.2.0/renderer/shaders/phong_reflection_shadow.py`

 * *Files identical despite different names*

### Comparing `jaxrenderer-0.1.3/renderer/shadow.py` & `jaxrenderer-0.2.0/renderer/shadow.py`

 * *Files identical despite different names*

### Comparing `jaxrenderer-0.1.3/renderer/shapes/capsule.py` & `jaxrenderer-0.2.0/renderer/shapes/capsule.py`

 * *Files identical despite different names*

### Comparing `jaxrenderer-0.1.3/renderer/shapes/cube.py` & `jaxrenderer-0.2.0/renderer/shapes/cube.py`

 * *Files identical despite different names*

### Comparing `jaxrenderer-0.1.3/renderer/types.py` & `jaxrenderer-0.2.0/renderer/types.py`

 * *Files identical despite different names*

### Comparing `jaxrenderer-0.1.3/renderer/utils.py` & `jaxrenderer-0.2.0/renderer/utils.py`

 * *Files identical despite different names*

### Comparing `jaxrenderer-0.1.3/renderer/value_checker.py` & `jaxrenderer-0.2.0/renderer/value_checker.py`

 * *Files identical despite different names*

### Comparing `jaxrenderer-0.1.3/PKG-INFO` & `jaxrenderer-0.2.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaxrenderer
-Version: 0.1.3
+Version: 0.2.0
 Summary: Jax implementation of rasterizer renderer.
 Home-page: https://github.com/JoeyTeng/jaxrenderer
 License: Apache-2.0
 Author: Joey Teng
 Author-email: joey.teng.dev@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 3 - Alpha
@@ -38,18 +38,21 @@
 
 - Native JAX implementation, supports `jit`, `vmap`, etc.
 - Lighting is computed in main camera's eye space; while in PyTinyrenderer it is computed in world space.
 - Texture specification is different: in PyTinyrenderer, the texture is specified in a flattened array, while in JAX Renderer, the texture is specified in a shape of (width, height, colour channels). A simple way to transform old specification to new specification is to use the convenient method `build_texture_from_PyTinyrenderer`.
 - Rendering pipeline is different. PyTinyrenderer renders one object at a time, and share zbuffer and framebuffer across one pass. This renderer first merges all objects into one big mesh in world space, then process all vertices together, then interpolates and rasterise and render. For fragment shading, this is done by sweeping each row in a for loop, and batch compute all pixels together. For computing a pixel, all fragments for that pixels are batch compute together, then mixed. This is more memory efficient and allows `vmap` batching as far as possible.
 - Shadowing within the same object / mesh is allowed. This is not possible in PyTinyrenderer, as it deliberately checks if the shadow comes from the same object; if so, it will not consider to draw a shadow there.
 - Quaternion (for specifying rotation/orientation) is in the form of `(w, x, y, z)` instead of `(x, y, z, w)` in PyTinyrenderer. This is for consistency with `BRAX`.
+- No clipping is performed. To ensure correct rendering of objects with vertices at or behind camera plane, homogeneous interpolation (Olano and Greer, 1997)[^1] is used to avoid the need of homogeneous division.
 - Fix bugs
   - Specular lighting was wrong, where it forgets to reverse the light direction vector.
 
+[^1]: Marc Olano and Trey Greer. 1997. Triangle Scan Conversion Using 2D Homogeneous Coordinates. In _Proceedings of the ACM SIGGRAPH/EUROGRAPHICS Workshop on Graphics Hardware (HWWS ’97)_. ACM, New York, NY, USA, 89–95.
+
 ## Roadmap
 
-- [ ] Correctly implement a proper clipping algorithm
 - [ ] Support double-sided objects
 - [ ] Profile and accelerate implementation
 - [ ] Differentiable rendering
 - [ ] Build a ray tracer as well
+- [ ] <s>Correctly implement a proper clipping algorithm</s>
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

