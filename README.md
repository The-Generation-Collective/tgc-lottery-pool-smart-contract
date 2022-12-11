# Smart Contract of TGC Lottery Pool - Backend Server

### What's good here ?

- A lottery pool with Polygon blockchain just for fun
- A winner of the lottery round shall be picked based on the `modulo operation` of :

1. hashed of the `current block timestamp` and `current number - tickets length`
2. the tickets length

### Smart Contract Deployment & Verification

- deploy and verify smart contract using thirdweb sdk with `npx thirdweb@latest release`

### Development

- (Adri addr)deployer address - `0x041ba5a08c590190Dbde1d9BfFEb8b7Bac980C5F`
- contract v1 (archive) - `0x2538081fF6C9cD48c0030E3C7d98f7Aa601B7143`
- contract v2 - ``

### Production

- (REXX deployer addr) deployer address - `0xf6b3ccE719f4A8Def331d94D67b1eEE2D093df4c`
- contract v1 (archive) - `0x18960C0B19Ba1983d960A653409Ca91F45C96738`
- contract v2 - ``

## Building the project

After any changes to the contract, run:

```bash
npm run build
# or
yarn build
```

to compile your contracts. This will also detect the [Contracts Extensions Docs](https://portal.thirdweb.com/contractkit) detected on your contract.

## Deploying Contracts

When you're ready to deploy your contracts, just run one of the following command to deploy you're contracts:

```bash
npm run deploy
```

## Releasing Contracts

If you want to release a version of your contracts publicly, you can use one of the followings command:

```bash
npm run release
```
