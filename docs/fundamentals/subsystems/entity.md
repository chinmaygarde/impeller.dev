# Entity

Location: `//impeller/entity`

Sits one level above `//impeller/renderer` and provides a framework for building
2D renderers. Most of the pipeline state objects generated from shaders authored
at build time reside in this framework. The render-pass optimization and
pass-rewriting framework also resides there. This allows authoring composable 2D
rendering optimizations (like collapsing passes, or, eliding them completely).
