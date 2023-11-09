# 🇩🇰 Rent Market

## Flow Diagram

```mermaid
flowchart TB
    subgraph RM[Rent Market]
        direction TB
        RegData[registered NFT list]
        RentData[rented NFT list]
        Balance[user balance list]

        RegisterProcess([register NFT process])
        RentProcess([rent NFT process])
        SettleProcess([settle fee process])
        WithdrawProcess([withdraw balance process])  
    end

    subgraph AC[Account]
        direction TB
        SO[Service Owner]
        MO[Market Owner]
        NO[NFT Owner]
    end

    subgraph CR[Cron Job]
        direction TB
        CP[Cron Process]
    end

    U[User]

    %% Register Process
    NO --> |"`**1**`"| RegisterProcess --> |"`**2**`"| RegData

    %% Rent Process
    U --> |"`**3**`"| RentProcess
    RegData --> |"`**4**`"| RentProcess --> |"`**5**`"| RentData

    %% Settle Process
    CP --> |"`**6**`"| SettleProcess
    RentData --> |"`**7**`"| SettleProcess --> |"`**8**`"| Balance

    %% Withdraw Process
    NO <--> |"`**9, 11**`"| WithdrawProcess
    Balance --> |"`**10**`"| WithdrawProcess
    WithdrawProcess --> |"`**11**`"| SO
    WithdrawProcess --> |"`**11**`"| MO

```

## Process

### **NFT Minting and Registration**

* The NFT token owner (NO) mints an NFT and registers it within the NFT contract (N).

### **Renting Process**

* The user (U) initiates the process by renting the NFT from the market contract (M), leading to the settlement of the NFT within the market contract.

### **Fee Distribution**

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

