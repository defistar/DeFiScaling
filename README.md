# DeFiScaling

https://ethereum.stackexchange.com/questions/71664/offchain-vs-sidechain-vs-statechannel

- On-chain

Something existing in the public blockchain.

- Side-chain

```
Something existing in the different public blockchain with observable relationships between chains like bridges. Cosmos and Polkadot are projects for bridging data between public blockchains.
```

- Off-chain

```
Something not visible on the public blockchain. But usually, inputs/deposits and outputs/withdrawals are observable in the public blockchain. Everything in the middle of input-output usually is not publicly observable. For example, 0x project allows traders to create limit orders without on-chain transaction by just signing order details. Market order executors will use this signature to proof to a smart contract that exchange is legal. As you may guess canceling of limit orders is made with on-chain transaction.
```

3.1. Payment channels

```
2-parties sign the latest state of the balances in the channel and can provide proofs and signatures to the smart contract at the end of the process. The main use case is micropayments, for example, you can pay for downloads per KB or pay for the vehicle per minute without fees for every transaction.

Also Lightning Network for Bitcoin as well as Raiden Network for Ethereum allow to pay over the hops and take fees. In the scheme A -> B -> C the B is one who can forward funds completely offchain in a trustless manner and also charge fees.
```

3.2. State channels

```
Same as payment channels but not only for balances. Potentially could be implemented any 2-party interaction even chess and sea battle.
```

3.2. Plasma

```
Same as payment channels but for multi-party interaction. Have a central operator who helps participants to interact. Have limitation to the ledger (usually as UTXO Bitcoin model) due possibility to proof to smart contract plasma operator's misbehavior.
```
