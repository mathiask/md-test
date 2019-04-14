# Test of GH_Pages, Syntax Highlighting and Embedded Diagrams
(see https://mathiask.github.io/md-test/)

A simple test
```js
var x = 42;
```
## Dot diagram
![DOT diagram](https://g.gravizo.com/svg?
digraph G {
    A -> B
    B -> A 
    A -> C 
}
)

## Class Diagram (minimal)
![minimal](https://g.gravizo.com/svg?
@startuml
A --> B
A -> C
@enduml
)

## Class Diagram
![Class diagram](https://g.gravizo.com/svg?
@startuml
class Player {
  x
}

Player --> GraphicsBoard

interface Board {
  p
  +m()
}
GraphicsBoard -> Board

note right: an interface

hide D members
hide D circle
GraphicsBoard --> D
@enduml
)

## Sequence Diagram
![Sequence diagram](https://g.gravizo.com/svg?
@startuml
  Alice -> Bob: synchronous call;
  Bob ->> C: asynchronous call;
@enduml
)
