---
description: Talk to avatar of AI model
---

# 🙍♀ AvaMe

<figure><img src="../.gitbook/assets/image.png" alt=""><figcaption></figcaption></figure>

* **Description**

Users can select their avatars and express motion or face with the avatars in avame.xyz service.

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
  * [https://avame-development.vercel.app](https://avame-development.vercel.app/)
* **GitHub**
  * [https://github.com/realbits-lab/avame](https://github.com/realbits-lab/avame)
* **Dework**
  * [https://app.dework.xyz/realbits/avame](https://app.dework.xyz/realbits/avame)
* **Discord**
  * [#avame](https://discord.com/channels/1049501409755811940/1054219044703707196)

