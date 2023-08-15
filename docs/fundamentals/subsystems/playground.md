# Playground

Location: `//impeller/playground`

When working with graphics APIs, it is often necessary to visually verify
rendering results as a specific feature is being worked upon. Moreover, it is
useful to attach frame debuggers or profilers to specific test cases. The
playground framework provides Google Test fixtures that open the current state
of various rendering related objects in a window in which rendering results can
be visualized, or, to which frame debuggers can be attached. Most Impeller
sub-frameworks that have a test harness also have a custom playground subclass.
This sub-framework is only meant to provide utilities for tests and will not be
compiled into any shipping binary.
