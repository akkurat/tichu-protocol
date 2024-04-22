# tichu-protocol
---
```mermaid
stateDiagram-v2
    [*] --> Round
    Round --> 8_Cards
    8_Cards --> All_Cards
    All_Cards --> Tichu_Before_Schupf
    Tichu_Before_Schupf --> Schupf
    Schupf --> Tichu?
    Tichu? --> One
    One --> Winner: Trick
    Winner --> Winner: Trick
    Winner --> End?: SecondLast?

    End? --> [*]: Team X >= 1000 pts
    End? --> Round : Noone >= 1000 ptx

```
