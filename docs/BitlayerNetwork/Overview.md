---
sidebar_position: 10
---

# Overview of Bitlayer V1

| Item | Value | Note |
| :--- | --- | --- |
| Gas token(Native token) | BTC | Come from Bitcoin chain through official bridge |
| Project token | [BTR](https://www.btrscan.com/address/0x0e4cf4affdb72b39ea91fa726d291781cbd020bf?tab=Transactions) | Not yet TGE |
| Networks info | refer to [Networks](./Networks.md) |  |
| Consensus | DPoSA | Stake BTR, the staking DAPP is under building |
| Block interval | 3 seconds |  |
| Block gasLimit | 40,000,000 | Can support more than `100 million` gas, and will increase capacity in time according to network congestion |
| Will block reorg? | Yes |  |
| Finality | very high probability safe with `15 blocks confirmations`; <br/>**absolutely safe** with `21 blocks confirmations` | refer to [About Finality](./AboutFinality.md) |
| EIP-1559 supported | Yes |  |
| Priority fee per gas requied | 0.1 gwei |  |
| Minimum gasPrice for legacy transaction | 0.100000007 gwei |  |
| Will base fee be burned? | No |  |
| EVM compatibility | Supported up to `Cancun` | But without opcode `PREVRANDAO`, `BLOBHASH`, and `BLOBBASEFEE`, <br/>do NOT support `Blob transaction` |
| Solidity version supported | ≤ 0.8.25 |  |
| Geth json-rpc compatibility | Fully support but with `eth_feeHistory` disabled | Can use `eth_feeHistory2` instead, <br/>because there's some issue for Metamask users when priority fee per gas is less than `1 gwei`, and we want to avoid our users spending unnecessary high fee. |
| Extra json-rpc | refer to [Json-RPC](./Json-RPC.md) |  |
| Some basic or important contracts | refer to [Contracts](./Contracts.md) |  |
