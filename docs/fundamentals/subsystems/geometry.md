# Geometry

Location: `//impeller/geometry`

All (or, most of) the math! This C++ mathematics library is used extensively by
Impeller and its clients. The reasonably interesting bit about this library is
that all types can be used interchangeably in device and host memory. Various
Impeller subsystems understand these types and can take care of packing and
alignment concerns w.r.t these types.
