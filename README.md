# ETCswap Swap Router Contracts

Smart contracts for combined V2 + V3 swap routing on Ethereum Classic.

Forked from [Uniswap Swap Router Contracts](https://github.com/Uniswap/swap-router-contracts). The `etcswap` branch contains ETC-specific `POOL_INIT_CODE_HASH` and build artifacts.

## Status: Reference / Deployed

The SwapRouter02 contract supports both V2 and V3 swaps in a single transaction. Deployed and immutable.

## ETC-Specific Changes (etcswap branch)

- `POOL_INIT_CODE_HASH` set to `0x7ea2da342810af3c5a9b47258f990aaac829fe1385a1398feb77d0126a85dbef`
- Build artifacts included for deployment verification

## Key Contracts

- **SwapRouter02.sol** — Combined V2 + V3 swap router
- **V2SwapRouter.sol** — V2-specific swap logic
- **V3SwapRouter.sol** — V3-specific swap logic
- **ApproveAndCall.sol** — Token approval and swap in one transaction

## Related Repos

- [v2-core](https://github.com/etcswap/v2-core) — V2 Factory and Pair contracts
- [v2-periphery](https://github.com/etcswap/v2-periphery) — V2 Router
- [sdks](https://github.com/etcswap/sdks) — TypeScript SDK monorepo (router-sdk package)

## Local Development

```bash
yarn install
npx hardhat compile
npx hardhat test
```
