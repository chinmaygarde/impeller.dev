# Image

Location: `//impeller/image`

The Impeller renderer works with textures whose memory is resident in device
memory. However, pending the migration of `//flutter/display_list` to graphics
package agnosticism and the subsequent migration of the image decoders to work
with the package agnostic types, there needs to be a way for tests and such to
decode compressed image data. This sub-framework provides that functionality.
This sub-framework is slated for removal and must not be used outside of tests.
