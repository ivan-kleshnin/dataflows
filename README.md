# Data flows of different web app architectures

> `active => passive`

> `any <- reactive`

#### jQuery (old school)

`DOM <- EventHandler => DOM`

#### Backbone / Ampersand

`DOM <- View => Model <- View => DOM`

#### Knockout
`DOM <- View (handlers) => ViewModel <- View (bindings) => DOM`

#### Flux / Flummox / ...
`Component => Action => Dispatcher <- Store <- Store (aggregate) <- Component`

#### Reflux
`Component => Action <- Store <- Store (aggregate) <- Component`

#### Baobab 
`Component => Action => State <- Facets <- Component`

#### Cycle
`User <- Computer <- VDOM <- User`
