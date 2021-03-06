# Test of GH_Pages, Syntax Highlighting and Embedded Diagrams
(see [https://mathiask.github.io/md-test/](https://mathiask.github.io/md-test/))

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
@startuml;
class A;
class B;
class C;
A --> B;
A -> C;
@enduml
)

## Class Diagram (complex, indirect)
![Class diagram](https://g.gravizo.com/source/svg/MAGIC_MARK1?https%3A%2F%2Fraw.githubusercontent.com%2Fmathiask%2Fmd-test%2Fmaster%2FREADME.md)
<details> 
<summary></summary>
MAGIC_MARK1
@startuml;
class Player {;
  x;
};

Player --> GraphicsBoard;

interface Board {;
  p;
  +m%28%29;
};
GraphicsBoard -> Board;

note right: an interface;

hide D members;
hide D circle;
GraphicsBoard --> D;
@enduml;
MAGIC_MARK1
</details>

## Sequence Diagram
![Sequence diagram](https://g.gravizo.com/svg?
@startuml;
  Alice -> Bob: synchronous call;
  Bob ->> C: asynchronous call;
@enduml
)
