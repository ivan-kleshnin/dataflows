# Frontend architectures overview

## Similarity table
<table>
  <tr>
    <th>jQuery</th>
    <th>Backbone</th>
    <th>React</th>
    <th>React Flux</th>
    <th>Baobab</th>
    <th>Cycle</th>
  </tr>
  <tr>
    <td>–</td><td>Model</td>
    <td>Component: state</td>
    <td>Store</td>
    <td>State</td>
    <td>Model</td>
  </tr>
  <tr>
    <td>–</td>
    <td>View</td>
    <td>Component: render</td>
    <td>Component</td>
    <td>Component</td>
    <td>View</td>
  </tr>
  <tr>
    <td>Event handler</td>
    <td>Event handler</td>
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

#### Flux / Flummox / ...
`Component => Action => Dispatcher <- Store <- Component`

#### Reflux
`Component => Action <- Store <- Component`

#### Baobab
`Component => Action => State <- Component`

#### Cycle
`Model <- View <- DOMUser <- Intent <- Model`
