---
description: Non-Fungible Token based ERC-721 interface
---

# NFT

We have 3 kinds of NFT.

* [rentNFT](https://github.com/realbits-lab/rent-market/blob/main/contracts/rentNFT.sol)
* [promptNFT](https://github.com/realbits-lab/rent-market/blob/main/contracts/promptNFT.sol)
* [paymentNFT](https://github.com/realbits-lab/rent-market/blob/main/contracts/paymentNFT.sol)

rentNFT is a general NFT smart contract. Most of NFT can use this open source.

promptNFT is a specialized NFT only for image gallery service. This not only supports ERC-721 interface, but also provides a encryption and decryption of prompt data.

paymentNFT is for service payment usage. This is based on rentNFT smart contract. Only different part is smart contract name.

{% embed url="https://github.com/realbits-lab/rent-market/tree/main/contracts" %}

