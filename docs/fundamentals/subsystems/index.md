# Subsystems

Impeller is a meta-framework. While a user of Impeller may choose to include the
whole enchilada (in `//impeller/:impeller`), the various sub-frameworks have
clearly defined responsibilities and adhere to a strict hierarchy.

Impeller itself may not depend on anything in `//flutter` except `//flutter/fml`
and `flutter/display_list`. FML is a base library for C++ projects and Impeller
implements the display list dispatcher interface to make it easy for Flutter to
swap the renderer with Impeller. Impeller is meant to be used by the Flow
(`//flutter/flow`) subsystem. Hence the name. The tessellator and geometry
libraries are exceptions - they unconditionally may not depend on anything from
`//flutter`.

This is an overview of the major sub-frameworks, their responsibilities, and,
relative states of completion.
