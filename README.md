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

#### Knockout + Model
`DOM <- View (handlers) => ViewModel <- Model <- View (bindings) => DOM`

#### Angular
TODO

## Generation Three

VirtualDOM

#### React
`Component <- Component (handler) => Component (state)`

#### Flux / Flummox / ...
`Component <- Action => Dispatcher <- Store <- Store (aggregate) <- Component`

#### Reflux
`Component <- Action <- Store <- Store (aggregate) <- Component`

#### Baobab 
`Component <- Action => State <- Facets <- Component`

#### Cycle
`User <- Computer <- User`
