# 🇩🇰 Rent Market

1. **NFT Minting and Registration**
   * The NFT token owner (NO) mints an NFT and registers it within the NFT contract (N).
2. **Renting Process**
   * The user (U) initiates the process by renting the NFT from the market contract (M), leading to the settlement of the NFT within the market contract.
3. **Fee Distribution**
   * Following the rental, the market contract (M) distributes the rent fee to the NFT token owner (NO), the market owner (MO), and the service owner (SO) as part of the fee-sharing process.

```mermaid
sequenceDiagram

actor U as User
participant N as NFT contract
participant M as Market contract
participant T as Token contract
participant S as Share contract

actor NO as NFT token owner
participant MO as Market owner
participant SO as Service owner

NO->>N: Mint NFT
NO->>M: Register NFT

U->>M: Rent NFT
M->>M: Settle NFT
M->>NO: Share rent fee (default 80%)
M->>MO: Share rent fee (default 10%)
M->>SO: Share rent fee (default 10%)

```
