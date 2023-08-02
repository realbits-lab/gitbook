---
description: AI 아바타와 대화하기
---

# 🏈 AvaMe

<figure><img src="../.gitbook/assets/image.png" alt="" width="375"><figcaption><p>아바타 화면</p></figcaption></figure>

* **설명**

사용자는 아바타 캐릭터를 선택하고 대화를 할 수 있습니다.

* **시퀀스 다이어그램**

```mermaid
sequenceDiagram

autonumber

participant U as 사용자
participant S as avame.xyz
participant M as 마켓 계약
participant O as NFT 소유자

U->>S: 아바타 대여 요청
S->>M: 수수료와 함께 아바타 NFT 대여
M->>S: 거래 응답
S->>U: 아바타 사용 허용
Note over U,O: 대여 기간 종료
M->>M: 대여 수수료 정산
M->>O: 대여 수수료 일부 이전
M->>S: 대여 수수료 일부 이전
M->>M: 대여 수수료 일부 이전


```

* **사이트**
  * [https://test.avame.xyz](https://test.avame.xyz/)
* **GitHub**
  * [https://github.com/realbits-lab/avame](https://github.com/realbits-lab/avame)