# Blobcat

Location: `//impeller/blobcat`

Concatenates shader blobs. This is primarily used by rendering backends that
don't have the notion of a shader library. In Impeller, all shaders are packaged
into a single library that contains a manifest of the shaders in the library
along with the pre-compiled shaders themselves. Unlike Metal, backends like
OpenGL ES and Vulkan don't have such a concept. For these backends,
`//impeller/blobcat` is used to create a single shader library to be packaged
with the engine.
