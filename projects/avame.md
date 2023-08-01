---
description: Talk to AI avatar
---

# 🙍♀ AvaMe

<figure><img src="../.gitbook/assets/image.png" alt="" width="375"><figcaption><p>Avatar screen</p></figcaption></figure>

* **Description**

Users can select avatar character and have a dialogue.

* **Sequence Diagram**

```mermaid
sequenceDiagram

autonumber

participant U as User
participant S as avame.xyz
participant M as Market Contract
participant O as NFT Owner

U->>S: Request to rent an avatar
S->>M: Rent avatar NFT with fee
M->>S: Response transaction
S->>U: Allow to use the avatar
Note over U,O: Rent duration finish
M->>M: Settle rent fee
M->>O: Transfer rent fee portion
M->>S: Transfer rent fee portion
M->>M: Transfer rent fee portion


```

* **Site**
  * [https://test.avame.xyz](https://test.avame.xyz/)
* **GitHub**
  * [https://github.com/realbits-lab/avame](https://github.com/realbits-lab/avame)

