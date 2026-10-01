# inadbehringer

```mermaid
---
config:
  theme: redux-color
  look: neo
---

swimlane-beta TB
  subgraph INAD
    Browse[Browse catalogue]
    Pay[Pay]
  end
  subgraph Geurt Janssen
    Pick[Pick items]
    Ship[Ship order]
  end
  subgraph Behringer
    Invoice[Raise invoice]
  end
  Browse --> Pay
  Pay --> Pick
  Pick --> Ship
  Pay --> Invoice

```
