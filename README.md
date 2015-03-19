# Frontend architectures overview

## Similarity table
<table>
  <tr><th>Backbone</th><th>Flux</th><th>Cycle</th></tr>
  <tr><td>Model</td><td>Store</td><td>Model</td></tr>
  <tr><td>View</td><td>Component</td><td>View</td></tr>
  <tr><td>Real DOM</td><td>[magic]</td><td>DOM User</td></tr>  
  <tr><td>Event handler</td><td>Action</td><td>Intent</td></tr>  
</table>

## Data flows

> `active => passive`

> `any <- reactive`

#### jQuery (old school)

`DOM <- EventHandler => DOM`

#### Backbone

`DOM <- View => Model <- View => DOM`

#### Flux
`Component => Action => Dispatcher <- Store <- Component`

#### Reflux
`Component => Action <- Store <- Component`

#### Baobab
`Component => Action => State <- Component`

#### Cycle
`Model <- View <- DOM <- Intent <- Model`
