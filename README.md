# inadbehringer

```mermaid
---
config:
  theme: redux-color
---


swimlane-beta TB
  subgraph INAD
    OrderLinesEntered([Order lines entered])
    TriggerType{Trigger type}
Released{Released?}
OrderReadyForBehringer[Order Ready For Behringer]
LaunchBehringerProgram[Launch Behringer program]
Stop([Stop])
  end
  subgraph Geurt Janssen
    Pick[Pick items]
    Ship[Ship order]
  end
  subgraph Behringer
    Invoice[Raise invoice]
  end
OrderLinesEntered --> TriggerType
TriggerType --> |Automatic trigger| Released
TriggerType --> |Manual tigger button or shortcut| OrderReadyForBehringer
Released --> |Not yet released| Stop 
OrderReadyForBehringer --> LaunchBehringerProgram
```
