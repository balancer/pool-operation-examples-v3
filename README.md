# Pool Operation Examples

A collection of example scripts for Balancer v3 pool operations configured to run on a local fork of Ethereum mainnet.

## Environment Setup

1. Ensure you have the latest version of foundry installed

```
foundryup
```

2. Clone this repo & install dependencies

```
git clone https://github.com/MattPereira/balancer-pool-operation-examples.git
cd balancer-pool-operation-examples
pnpm install
```

3. Add a `MAINNET_RPC_URL` to a `.env` file

```
MAINNET_RPC_URL=
```

## Hardhat scripts

```
npx hardhat run scripts/hardhat/<path_to_script>
```

## Foundry scripts

```
forge script scripts/foundry/<path_to_script> --fork-url mainnet
```

## Add Liquidity

<table>
  <tr>
    <th>Kind</th>
    <th>Typescript</th>
    <th>Solidity</th>
  </tr>
  <tr>
    <th rowspan="2">Unbalanced</th>
    <td><a href="scripts/hardhat/add-liquidity/addLiquidityUnbalanced.ts">addLiquidityUnbalanced.ts</a></td>
    <td><a href="scripts/foundry/add-liquidity/AddLiquidityUnbalanced.s.sol">AddLiquidityUnbalanced.s.sol</a></td>
  </tr>
  <tr>
    <td><a href="scripts/hardhat/add-liquidity/addLiquidityUnbalancedToERC4626.ts">addLiquidityUnbalancedToERC4626.ts</a></td>
    <td><a href="scripts/foundry/add-liquidity/addLiquidityUnbalancedToERC4626.s.sol">AddLiquidityUnbalancedToERC4626.s.sol</a></td>
  </tr>
    <tr>
    <th rowspan="2">Proportional</th>
    <td><a href="scripts/hardhat/add-liquidity/addLiquidityProportional.ts">addLiquidityProportional.ts</a></td>
    <td><a href="scripts/foundry/add-liquidity/AddLiquidityProportional.s.sol">AddLiquidityProportional.s.sol</a></td>
  </tr>
  <tr>
    <td><a href="scripts/hardhat/add-liquidity/addLiquidityProportionalToERC4626.ts">addLiquidityProportionalToERC4626.ts</a></td>
    <td><a href="scripts/foundry/add-liquidity/AddLiquidityProportionalToERC4626.s.sol">AddLiquidityProportionalToERC4626.s.sol</a></td>
  </tr>
</table>

## Remove Liquidity

<table>
  <thead>
    <th>Kind</th>
    <th>Typescript</th>
    <th>Solidity</th>
  </thead>
  <tbody>
  <tr>
    <th>SingleTokenExactIn</th>
    <td><a href="scripts/hardhat/remove-liquidity/removeLiquiditySingleTokenExactIn.ts">removeLiquiditySingleTokenExactIn.ts</a></td>
    <td><a href="scripts/foundry/remove-liquidity/RemoveLiquiditySingleTokenExactIn.s.sol">RemoveLiquiditySingleTokenExactIn.s.sol</a></td>
  </tr>
    <tr>
    <th>SingleTokenExactOut</th>
    <td><a href="scripts/hardhat/remove-liquidity/removeLiquiditySingleTokenExactOut.ts">removeLiquiditySingleTokenExactOut.ts</a></td>
    <td><a href="scripts/foundry/remove-liquidity/RemoveLiquiditySingleTokenExactOut.s.sol">RemoveLiquiditySingleTokenExactOut.s.sol</a></td>
  </tr>
    <tr>
    <th style="text-align: left" rowspan="2">Proportional</th>
    <td><a href="scripts/hardhat/remove-liquidity/removeLiquidityProportional.ts">removeLiquidityProportional.ts</a></td>
    <td><a href="scripts/foundry/remove-liquidity/RemoveLiquidityProportional.s.sol">RemoveLiquidityProportional.s.sol</a></td>
  </tr>
  <tr>
    <td><a href="scripts/hardhat/remove-liquidity/removeLiquidityProportionalToERC4626.ts">removeLiquidityProportionalToERC4626.ts</a></td>
    <td><a href="scripts/foundry/remove-liquidity/RemoveLiquidityProportionalToERC4626.s.sol">RemoveLiquidityProportionalToERC4626.s.sol</a></td>
  </tr>
  </tbody>
</table>

## Swap

<table>
  <tr>
    <th>Kind</th>
    <th>TypeScript</th>
    <th>Solidity</th>
  </tr>
  <tr>
    <th>GivenIn</th>
    <td>swapSingleTokenExactIn.ts</td>
    <td><a href="scripts/foundry/swap/SwapSingleTokenExactIn.s.sol">SwapSingleTokenExactIn.s.sol</a></td>
  </tr>
  <tr>
    <th>GivenOut</th>
    <td>swapSingleTokenExactOut.ts</td>
    <td><a href="scripts/foundry/swap/SwapSingleTokenExactOut.s.sol">SwapSingleTokenExactOut.s.sol</a></td>

</table>
