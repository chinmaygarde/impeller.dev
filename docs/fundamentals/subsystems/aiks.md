# Aiks

Location: `//impeller/aiks`

Aiks is Skia in the upside-down.

Aiks wraps `//impeller/entity` into an API that resembles Skia. This makes it
easy to mechanically replace Skia calls with their Impeller counterparts even
though the `//impeller/entity` framework API is different from Skia. This
presence of this sub-framework is probably short-lived as integration of
Impeller into Flutter should likely happen via a custom Display List
implementation in `//impeller/display_list`. The roadblocks to this today are
graphics package agnosticism in the Display List interface.
