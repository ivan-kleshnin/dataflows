# Dataflows of web app architectures

> `active => passive`

> `any <- reactive`

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

Including **React** scheme...

`[DOM <-] Component (handler) => Action => Dispatcher <- Store <- Store (aggregate) <- Component (VDOM) [=> DOM]`

#### Reflux

Including **React** scheme...

`[DOM <-] Component (handler) => Action <- Store <- Store (aggregate) <- Component (VDOM) [=> DOM]`

#### Baobab 

Including **React** scheme...

`[DOM <-] Component (handler) => Action => State <- Facets <- Component (VDOM) [=> DOM]`

#### Cycle

Basic

`[DOM <-] Computer (VDOM) [=> DOM]`

Advanced

`[DOM <-] Intent <- Model <- View (VDOM) [=> DOM]`
