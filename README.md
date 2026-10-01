# inadbehringer

```mermaid
---
config:
  theme: redux
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
[![](https://mermaid.ink/img/pako:eNp1U01v2zAM_SsETy2QBPlO7EOHdt2GDm1XpDnNzkGxWVtYLBkytTZN8t8nW_nosOxCkI98JPUIbTDRKWGI1assVkJRe0ksYH4TK4DKLjMjyhzuHq9vawDgh0nJ3EtF1RfFZCi9iBoIVjUG5MHFpa-eG5llZObrkjZ7H9gFu1jNaEWionRzcD45sGk1I5Guv2pzQ7mRylH2ExocXAKOmUWs7oVVSX5Enox2KxeRh0-VUPqEYzyzLi-i2vo1SaV_PfYbWcPwXaiqIuXf8SSTX1FtQDIV1cKjz7kso9qArhdcnGt2XMBT7tRvLROKZkJWBNJHJ-I_6kK7ffVRxVh9CJrk9tqyLgTLBNintnCQ9Ez1g1BWrID9LZaWWSu3PlS5NpxY3sL5G5wO5vs8aoY1MZg9uoVaUPjfCRvS-VNhCzMjUwzZWGphQaYQdYibWpYYOaeCYgyd6wSxb22lX2OM1c4RS6F-al0cuEbbLMfwRawqF9kyFUy3UjRTDqhxQpP5rK1iDHvBuGmC4QbfMBxMBp1-f9IbTMaD8bgbTFu4xrA_7QTd6XAY9IJerz_pjnYtfG-mdjvBcDjtDl1iNA0Go9GohZRK1ubBf6pEqxeZ4e4P1O4umQ?type=png)](https://mermaid.ai/live/edit#pako:eNp1U01v2zAM_SsETy2QBPlO7EOHdt2GDm1XpDnNzkGxWVtYLBkytTZN8t8nW_nosOxCkI98JPUIbTDRKWGI1assVkJRe0ksYH4TK4DKLjMjyhzuHq9vawDgh0nJ3EtF1RfFZCi9iBoIVjUG5MHFpa-eG5llZObrkjZ7H9gFu1jNaEWionRzcD45sGk1I5Guv2pzQ7mRylH2ExocXAKOmUWs7oVVSX5Enox2KxeRh0-VUPqEYzyzLi-i2vo1SaV_PfYbWcPwXaiqIuXf8SSTX1FtQDIV1cKjz7kso9qArhdcnGt2XMBT7tRvLROKZkJWBNJHJ-I_6kK7ffVRxVh9CJrk9tqyLgTLBNintnCQ9Ez1g1BWrID9LZaWWSu3PlS5NpxY3sL5G5wO5vs8aoY1MZg9uoVaUPjfCRvS-VNhCzMjUwzZWGphQaYQdYibWpYYOaeCYgyd6wSxb22lX2OM1c4RS6F-al0cuEbbLMfwRawqF9kyFUy3UjRTDqhxQpP5rK1iDHvBuGmC4QbfMBxMBp1-f9IbTMaD8bgbTFu4xrA_7QTd6XAY9IJerz_pjnYtfG-mdjvBcDjtDl1iNA0Go9GohZRK1ubBf6pEqxeZ4e4P1O4umQ)
