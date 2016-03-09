# Dataflows

> `active => passive`

> `emitter <- reactive`

Time flows from left to right.<br/>
Arrows point from dependent to dependency.

Active "thing" requires passive "thing" and invokes it's behavior.<br/>
Reactive "thing" requires emitter "thing" and subscribes to it's events.

## Generation One

Manual DOM mutations

#### jQuery

`DOM <- EventHandler => DOM`

#### Backbone / Ampersand

`DOM <- View => Model <- View => DOM`

## Generation Two

Automatic DOM mutations

#### Knockout

`[DOM <-] View (handlers) => ViewModel <- View (bindings) [=> DOM]`

With Model

`[DOM <-] View (handlers) => ViewModel <- Model <- ViewModel <- View (bindings) [=> DOM]`

#### Angular

TODO

## Generation Three

Virtual DOM

#### React

`[DOM <-] Component (handler) => Component (state) <- Component (VDOM) [=> DOM]`

#### Flux / Flummox / ...

`[DOM <-] Component (handler) => Action => Dispatcher <- Store <- Store (agg.) <- Component (VDOM) [=> DOM]`

Also includes **React** scheme.

`agg.` means `aggregate`

#### Reflux

`[DOM <-] Component (handler) => Action <- Store <- Store (agg.) <- Component (VDOM) [=> DOM]`

Also includes **React** scheme.

`agg.` means `aggregate`

#### Baobab 

Including **React** scheme...

`[DOM <-] Component (handler) => Action => State <- Facets <- Component (VDOM) [=> DOM]`

#### Cycle

Basic

`[DOM <-] Computer (VDOM) [=> DOM]`

Advanced

`[DOM <-] Intent <- Model <- View (VDOM) [=> DOM]`

## Links

[reactive-polyglot](https://github.com/ivan-kleshnin/reactive-polyglot) – FRP libraries / langs compared
