# Data flows of different web app architectures

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

`DOM <- View (handlers) => ViewModel <- View (bindings) => DOM`

With Model

`DOM <- View (handlers) => ViewModel <- Model <- ViewModel <- View (bindings) => DOM`

#### Angular

TODO

## Generation Three

Virtual DOM

#### React

`Component (VDOM) <- Component (handler) => Component (state) <- Component (VDOM)`

#### Flux / Flummox / ...

Including **React** scheme...

`Component <- Action => Dispatcher <- Store <- Store (aggregate) <- Component`

#### Reflux

Including **React** scheme...

`Component <- Action <- Store <- Store (aggregate) <- Component`

#### Baobab 

Including **React** scheme...

`Component <- Action => State <- Facets <- Component`

#### Cycle

Basic

`User <- Computer <- User`

Advanced

`View <- Intent <- Model <- View`
