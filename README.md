# text-diagram

Text Diagram is a web tool for drawing UML sequence diagram in pure text.

Original: https://github.com/weidagang/text-diagram


## Input

```txt
object April Todd Monad
April->April: Prepare food for lunch.
space 5
note left of April: Lunch is ready.
April->Todd: Todd, what are you doing?
note right of Todd: @_@
Todd->April: Well...\nI'm programming.
space 5
April->Monad: How about you?
Monad->April: I'm reading book.
April->Monad: Good boy!
note right of Monad: ^_^
```

## Output

```txt
                +-------+                       +-------+               +-------+
                | April |                       | Todd  |               | Monad |
                +-------+                       +-------+               +-------+
                    |                               |                       |
                    | Prepare food for lunch.       |                       |
                    |------------------------       |                       |
                    |                       |       |                       |
                    |<-----------------------       |                       |
                    |                               |                       |
                    |                               |                       |
                    |                               |                       |
                    |                               |                       |
                    |                               |                       |
------------------\ |                               |                       |
| Lunch is ready. |-|                               |                       |
|-----------------| |                               |                       |
                    |                               |                       |
                    | Todd, what are you doing?     |                       |
                    |------------------------------>|                       |
                    |                               | ------------------\   |
                    |                               |-| Programming @_@ |   |
                    |                               | |-----------------|   |
                    |                               |                       |
                    |                       Well... |                       |
                    |              I'm programming. |                       |
                    |<------------------------------|                       |
                    |                               |                       |
                    |                               |                       |
                    |                               |                       |
                    |                               |                       |
                    |                               |                       |
                    |                               |                       |
                    | How about you?                |                       |
                    |------------------------------------------------------>|
                    |                               |                       |
                    |                               |     I'm reading book. |
                    |<------------------------------------------------------|
                    |                               |                       |
                    | Good boy!                     |                       |
                    |------------------------------------------------------>|
                    |                               |                       | ----------------\
                    |                               |                       |-| I'm so happy. |
                    |                               |                       | | ^_^           |
                    |                               |                       | |---------------|
                    |                               |                       |

```