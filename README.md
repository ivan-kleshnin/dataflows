## Architecture
<table>
  <tr><th>Flux</th><th>Cycle</th></tr>
  <tr><td>Store</td><td>Model</td></tr>
  <tr><td>Component</td><td>View</td></tr>
  <tr><td>[magic]</td><td>DOM User</td></tr>  
  <tr><td>Action</td><td>Intent</td></tr>  
</table>

* In CycleJS there can be more nodes.

## Data flows

### Legend

> `=>` active

> `<-` reactive

#### Flux
  Component => Action => Dispatcher <- Store <- Component

#### Reflux
  Component => Action <- Store <- Component

#### Baobab
  Component => Action => State <- Component

#### Cycle
  Model <- View <- Intent <- Model
