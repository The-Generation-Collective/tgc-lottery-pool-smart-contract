<div align="center">
  <a href="https://tgcollective.xyz">
    <img src="https://www.tgcollective.xyz/_next/image?url=%2F_next%2Fstatic%2Fmedia%2Frexxie-banner.227d942b.webp&w=3840&q=75" alt="tgc_fam" width="800" height="200">
  </a>
  <h3 align="center">Smart Contract of TGC Lottery Pool - Smart Contract </h3>
  <h3 align="center">Created by: <a href="https://github.com/ass77">ass77</a></h3>
</div>

### What's good here ?

- This is a smart contract for a lottery pool on any EVM-compatible blockchains. The contract defines various parameters such as the ticket price, maximum number of tickets per round, and commission taken per ticket. It also has a duration for each round. The contract allows users to buy tickets, check their winnings, and withdraw their winnings if they are the winner. The lottery operator can also withdraw their commission and draw a winner at the end of the round. If the lottery is not expired, users can refund their tickets. The contract uses a random number generated from the block hash and timestamp to determine the winner. The contract also has various access control modifiers to ensure that only the lottery operator can perform certain functions.

- The winners (top 3) of the lottery round shall be picked based on the `modulo operation` of :

#### Top 3 Prizes

- number 1 prize = 60% from the total prize pool
- number 2 prize = 25% from the total prize pool
- number 3 prize = 15% from the total prize pool

1. hashed of the `current block timestamp` and `current number - tickets length`
2. the tickets length
3. the winners odds shall increased based on how many REXX NFT they are holding!

- if the user has `1 to 3 REXX NFT`, increase the odds by `2%` AKA `TIER 1 REXX`
- if the user has `4 to 6 REXXNFT`, increase the odds by `6%` AKA `TIER 2 REXX`
- if the user has `7 REXX NFT`, increase the odds by `10%` AKA `TIER 3 REXX`

## How To

### Build the project

After any changes to the contract, run:

```bash
npm run build
```

to compile your contracts. This will also detect the [Contracts Extensions Docs](https://portal.thirdweb.com/contractkit) detected on your contract.

### Deploying Contracts

When you're ready to deploy your contracts, just run one of the following command to deploy you're contracts:

```bash
npm run deploy
```

### Releasing Contracts

If you want to release a version of your contracts publicly, you can use one of the followings command:

```bash
npm run release
```
