# Toolkit

Location: `//impeller/toolkit`

Contains Impeller agnostic toolkits that provide more ergonomic  wrappers around
certain APIs like EGL. Toolkits must be dependency free so that an external
component using a toolkit doesn't have to pull in a significant portion of
Impeller itself.
