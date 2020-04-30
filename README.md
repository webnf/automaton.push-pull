# automaton.push-pull

    In the beginning there was normal order.
             And as nobody was there to hear it,
                   no tree was falling.

This library is about bringing lazy evaluation together with event
receivers, while being able to work in variable increments and have
full visibility.

It is modelled after cell programming and implements an interpreter
for formulas + dependencies. Compared to other cell libraries, the
interpreter allows to retain full visibility into the dependency graph
and intermittent memoization, and also to step the calculation state
for time slicing or debugging purposes. Its primary concern is
skipping recalculation of unchanged results (thus the `Formula`
abstraction, which promises to be pure), therefore event generation
can be cheaply added by traversing the dependency graph.

This README is vaporware, right now, but there is work-in-progress to
publish the interpreter for this.
