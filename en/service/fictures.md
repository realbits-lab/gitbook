---
description: Image NFT gallery service
---

# 🖼 Fictures

## Description

User can draw image using prompt with generative AI technology. User can mint NFT with the image.

User can generate and draw images with prompt text. Then, if desired, the image can be published as NFT with encrypted prompt data.

Whether minting is done or not, if user select to post image, image will be posted on service site. A minting image would not display the prompt to the user.

When the user wants to see the prompt, user would have to pay a token and see the prompt for a limited time (perhaps one day). When prompt duration ends, prompt fee will be shared with NFT owner, service owner, and market owner by smart contract.

<div data-full-width="false">

<figure><img src="../.gitbook/assets/image (4).png" alt="" width="188"><figcaption><p>Image NFT</p></figcaption></figure>

</div>

## Service Sequence Diagram

```mermaid
sequenceDiagram

autonumber

participant U as User
participant S as fictures.xyz
participant M as Market Contract
participant O as NFT Owner

U->>S: Request to rent an prompt
S->>M: Rent prompt NFT with fee
M->>S: Response transaction
S->>U: Allow to see the prompt
Note over U,O: Rent duration finish
M->>M: Settle rent fee
M->>O: Transfer rent fee portion
M->>S: Transfer rent fee portion
M->>M: Transfer rent fee portion
```

## **Site**

* [https://test.fictures.xyz](https://test.fictures.xyz/)

## **GitHub**

* [https://github.com/realbits-lab/prompt-nft](https://github.com/realbits-lab/prompt-nft)
