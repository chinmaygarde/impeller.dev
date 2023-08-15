# Typographer

Location: `//impeller/typographer`

Contains a backend agnostic interface for rendering typefaces. While Impeller does **not** do any text layout or shaping, it does render shaped glyph runs. The application specifies these glyph runs to Impeller using the Typographer subsystem.

## Typographer Backend

Location: `//impeller/typographer/backend`

Contains code that interfaces with an underlying (usually platform-specific)
library or toolkit to render glyphs in typefaces into texture atlases. Impeller
will then reference these glyphs when rendering shaped glyph runs. No Impeller
sub-frameworks may depend on these targets. There may be multiple typographer
backends.
