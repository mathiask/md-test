#Test of GH_Pages, Syntax Highlighting and Embedded Diagrams
(see https://mathiask.github.io/md-test/)

A simple test
```js
var x = 42;
```
## Dot diagram
![DOT diagram](https://g.gravizo.com/svg?
digraph G {
    // rankdir=LR
    ordering=out
    A -> B
    B -> A [label=back]
    A -> C [style=dotted]
}
)

## Class Diagram
![Class diagram](https://g.gravizo.com/svg?
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
B --> D
)

## Sequence Diagram
![Sequence diagram](https://g.gravizo.com/svg?
  Alice -> Bob: synchronous call
  Alice ->> Bob: asynchronous call
)
