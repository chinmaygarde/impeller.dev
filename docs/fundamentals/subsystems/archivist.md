# Archivist

Location: `//impeller/archivist`

Allows persisting objects to disk as performantly as possible (usually on a
background thread). The framework is meant to be used for storing frame
meta-data and related profiling/instrumentation information. Collection of
information should succeed despite process crashes and retrieval of traces must
not use inordinate amounts of time or memory (which usually leads to crashes).
