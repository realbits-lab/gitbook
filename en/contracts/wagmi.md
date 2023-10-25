---
description: Blockchain WEB3 JavaScript (TypeScript) library
---

# WAGMI

* JavaScript (TypeScript) package library for blockchain
* [React](https://wagmi.sh/react/getting-started) main libraries.
  * [useAccount](https://wagmi.sh/react/hooks/useAccount)
    * Hook for accessing account data and connection status.
  * [useBalance](https://wagmi.sh/react/hooks/useBalance)
    * Hook for fetching balance information for Ethereum or ERC-20 tokens.
  * [useConnect](https://wagmi.sh/react/hooks/useConnect)
    * Hook for connecting to account with connectors.
  * [useContractRead](https://wagmi.sh/react/hooks/useContractRead)
    * Hook for calling a read method on a Contract.
  * [useContractWrite](https://wagmi.sh/react/hooks/useContractWrite)
    * Hook for calling a write method on a Contract.
  * [useNetwork](https://wagmi.sh/react/hooks/useNetwork)
    * Hook for accessing network data, such as current connected chain and [connector chains](https://wagmi.sh/react/connectors/injected#chains-optional).
  * [useWaitForTransaction](https://wagmi.sh/react/hooks/useWaitForTransaction)
    * Hook for declaratively waiting until transaction is processed. Pairs well with `[useContractWrite](<https://wagmi.sh/react/hooks/useContractWrite>)` and `[useSendTransaction](<https://wagmi.sh/react/hooks/useSendTransaction>)`.
