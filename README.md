# Web app architectures. Overview

## Similarity table
<table>
  <tr>
    <th>jQuery</th>
    <th>Backbone</th>
    <th>Knockout</th>
    <th>React</th>
    <th>React Flux</th>
    <th>Baobab</th>
    <th>Cycle</th>
  </tr>
  <tr>
    <td>–</td>
    <td>Model</td>
    <td>ViewModel (Observables)</td>
    <td>Component: state</td>
    <td>Store</td>
    <td>State</td>
    <td>Model</td>
  </tr>
  <tr>
    <td>–</td>
    <td>View</td>
    <td>View (HTML with data-bind attrs)</td>
    <td>Component: render</td>
    <td>Component</td>
    <td>Component</td>
    <td>View</td>
  </tr>
  <tr>
    <td>Event handler</td>
    <td>Event handler</td>
    <td>Event Handler (declaratively attached)</td>
    <td>Component: event handler</td>
    <td>Action</td>
    <td>Action</td>
    <td>Intent</td>
  </tr>  
</table>

## Data flows

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
