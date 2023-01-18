
Grant Proposal | [386 - Fair Auction Launch System For Casper](https://portal.devxdao.com/public-proposals/386)
------------ | -------------
Milestone | 1:3
Milestone Titles | Liquidity Transformer (50 Day Fair Auction & Lockup Contract)<br>Advanced ERC-20 Token Example (WiseToken)<br>Synthetic Network Token (Synthetic Casper for CSPR:SCSPR Pair)
OP | CaptainBernardo
Reviewer | Muhammet Kara

# Milestone Details
The review will cover the first 3 milestones set forth below.

## Details & Acceptance Criteria

**Details of what will be delivered in milestones:**

This is a translation of https://github.com/wise-foundation/wise-token-contracts/blob/master/contracts/LiquidityTransformer.sol - This contract allows users to execute a 50 day fair auction with a set amount of supply equally distributed across all days (random supply/oracle functionality from the original contract is being removed) - Customers can purchase tokens for certain days After the auction ends, the customers receive their token allocations and all CSPR in the purse is staked to the AMM as a synthetic CSPR <-> ERC20 token pair The liquidity tokens received by the contract are then burned - This contract interops with milestone 2 and 3 deliverables Examples, Test & Documentation

---
This is a translation of https://github.com/wise-foundation/wise-token-contracts/blob/master/contracts/WiseToken.sol - The advanced ERC20 token that interops with the auction contract https://github.com/wise-foundation/wise-token-contracts/blob/master/contracts/LiquidityToken.sol - This allows LP token staking for special pairs on the AMM https://github.com/wise-foundation/wise-token-contracts/blob/master/contracts/StakingToken.sol - This allows lockup staking of the token, most of the functionality here is optional to other users https://github.com/wise-foundation/wise-token-contracts/blob/master/contracts/ReferralToken.sol - This allows the calculation of referral fees https://github.com/wise-foundation/wise-token-contracts/blob/master/contracts/Snapshot.sol - Daily snapshot functionality for future oracles, liquidity guard in low liquidity situations will be disabled https://github.com/wise-foundation/wise-token-contracts/blob/master/contracts/Helper.sol - Time calculation functions This set of contracts will create a ERC20 with special AMM aware functionality such as liquidity pool staking (for yield farming), some optional wise specific functionality (time base stakes), and some token sale functionality (referral functionality) This ERC20 allows the auction contract to do the issuance Examples, Tests & Documentation

---
This is a translation of https://github.com/wise-foundation/wise-token-contracts-bsc/blob/master/contracts/SBNB.sol - SCSPR will take CSPR from the auction and deposit/withdraw from a SCSPR <-> WCSPR pair collateralized by the CSPR from the auction SCSPR was added to the BSC version of this auction contract as an upgrade that allows part of the locked up treasury (exactly 50% in the worse case scenario) to be accessed due to portions of CSPR becoming dead in the liquidity pool due to transaction fees and other things (this inefficiency was identified in the Ethereum implementation). SCSPR also gates the amount of CSPR that can effect the ERC20 liquidity pool and prevents certain types of liquidity attacks aimed to drain all the ERC20 out of the system. Examples, Tests & Documentation

**Acceptance criteria:**

- Token issuer can create a contract with a supply, duration, and specific liquidity pair that will be targeted.
- Users can send this contract tokens every day to bid on the price of the token.
- Token supply is using the average price per day.
- Testing work
- Anyone can deploy an example
---
- Tokens can pay out referrals (default 1%)
- Tokens can be staked and pay out (default 3%) more tokens
- Tests work
- Anyone can deploy an example
---
- SCSPR allows for arbitrage within a SCPSR <-> WCSPR pair.
- Tests work
- Anyone can deploy an example

**Additional notes regarding submission from OP:**

These 3 milestone submissions are split between these two repos with mutual dependencies
Milestone 1 is located at liquidity-transformer/LiquidityTransformer/LiquidityTransformer
Milestone 2 is located in stakeable-token
Milestone 3 is located in liquidity-transformer/scspr/SCSPR/scspr

## Milestone Submission

The following milestone assets/artifacts were submitted for review:

Repository | Revision Reviewed
------------ | -------------
https://github.com/Rengo-Labs/CasperLabs-StakeableToken | 536e4af
https://github.com/Rengo-Labs/CasperLabs-LiquidityTransformer | 136c61d

In addition to the repositories above, the following assets/artifacts were also included as dependencies in the review:

Repository | Revision Reviewed
------------ | -------------
https://github.com/Rengo-Labs/CasperLabs-UniswapV2-Core | 3950019
https://github.com/Rengo-Labs/CasperLabs-UniswapV2-Router | a546970


# Install & Usage Testing Procedure and Findings

The reviewer successfully built and deployed the project on the Casper TestNet by following the instructions on the root-level and subdirectory-level READMEs of the repositories. All of the build and test operations were carried out on a Gitpod machine with Ubuntu 20.04 LTS operating system.

Please note that this result was achieved after many encountered errors and issues being reported to the OP, and then OP fixing them. This period took quite a while, causing the review to pass the anticipated deadline by far.

## Build Log
```bash
$ make build-all
make build-contract
make[1]: Entering directory '/workspace/CasperLabs-LiquidityTransformer'
cargo build --release -p liquidity_transformer -p scspr -p session-code-lt -p session-code-scspr --target wasm32-unknown-unknown
warning: patch for the non root package will be ignored, specify patch at the workspace root:
package:   /workspace/CasperLabs-LiquidityTransformer/liquidity_transformer/liquidity_transformer_crate/Cargo.toml
workspace: /workspace/CasperLabs-LiquidityTransformer/Cargo.toml
warning: patch for the non root package will be ignored, specify patch at the workspace root:
package:   /workspace/CasperLabs-LiquidityTransformer/liquidity_transformer/liquidity_transformer_tests/Cargo.toml
workspace: /workspace/CasperLabs-LiquidityTransformer/Cargo.toml
    Finished release [optimized] target(s) in 0.38s
make[1]: Leaving directory '/workspace/CasperLabs-LiquidityTransformer'
cd ../CasperLabs-UniswapV2-Core/erc20/ && make build-contract
make[1]: Entering directory '/workspace/CasperLabs-UniswapV2-Core/erc20'
cargo build --release -p erc20 --target wasm32-unknown-unknown
info: syncing channel updates for 'nightly-2022-01-13-x86_64-unknown-linux-gnu'
info: latest update on 2022-01-13, rust version 1.60.0-nightly (1bd4fdc94 2022-01-12)
info: downloading component 'cargo'
info: downloading component 'rust-std'
info: downloading component 'rustc'
info: installing component 'cargo'
info: installing component 'rust-std'
info: installing component 'rustc'
warning: unused imports: `BlockTime`, `ContractHash`
 --> erc20/src/erc20.rs:8:49
  |
8 |     system::mint::Error as MintError, ApiError, BlockTime, ContractHash, ContractPackageHash, Key,
  |                                                 ^^^^^^^^^  ^^^^^^^^^^^^
  |
  = note: `#[warn(unused_imports)]` on by default

warning: unused import: `hex::encode`
  --> erc20/src/erc20.rs:13:5
   |
13 | use hex::encode;
   |     ^^^^^^^^^^^

warning: unused imports: `hash_message`, `keccak256`
  --> erc20/src/erc20.rs:14:17
   |
14 | use renvm_sig::{hash_message, keccak256};
   |                 ^^^^^^^^^^^^  ^^^^^^^^^

warning: `erc20` (lib) generated 3 warnings
    Finished release [optimized] target(s) in 0.52s
wasm-strip target/wasm32-unknown-unknown/release/erc20-token.wasm 2>/dev/null | true
make[1]: Leaving directory '/workspace/CasperLabs-UniswapV2-Core/erc20'
cd ../CasperLabs-UniswapV2-Core/factory/ && make build-contract
make[1]: Entering directory '/workspace/CasperLabs-UniswapV2-Core/factory'
cargo build --release -p factory --target wasm32-unknown-unknown
warning: Patch `renvm-sig v0.1.1 (https://github.com/Scytalelabs-official/CasperLabs-renvm-sig.git?branch=main#bb97d895)` was not used in the crate graph.
Check that the patched package version and available features are compatible
with the dependency requirements. If the patch has a different version from
what is locked in the Cargo.lock file, run `cargo update` to use the new
version. This may also occur with an optional dependency that is not enabled.
    Finished release [optimized] target(s) in 0.49s
wasm-strip target/wasm32-unknown-unknown/release/factory.wasm 2>/dev/null | true
make[1]: Leaving directory '/workspace/CasperLabs-UniswapV2-Core/factory'
cd ../CasperLabs-UniswapV2-Core/flashswapper/ && make build-contract
make[1]: Entering directory '/workspace/CasperLabs-UniswapV2-Core/flashswapper'
cargo build --release -p flashswapper --target wasm32-unknown-unknown
warning: Patch `renvm-sig v0.1.1 (https://github.com/Scytalelabs-official/CasperLabs-renvm-sig.git?branch=main#bb97d895)` was not used in the crate graph.
Check that the patched package version and available features are compatible
with the dependency requirements. If the patch has a different version from
what is locked in the Cargo.lock file, run `cargo update` to use the new
version. This may also occur with an optional dependency that is not enabled.
    Finished release [optimized] target(s) in 0.48s
wasm-strip target/wasm32-unknown-unknown/release/flashswapper-token.wasm 2>/dev/null | true
make[1]: Leaving directory '/workspace/CasperLabs-UniswapV2-Core/flashswapper'
cd ../CasperLabs-UniswapV2-Core/pair/ && make build-contract
make[1]: Entering directory '/workspace/CasperLabs-UniswapV2-Core/pair'
cargo build --release -p pair --target wasm32-unknown-unknown
warning: unused import: `BlockTime`
  --> pair/src/pair.rs:13:29
   |
13 |     runtime_args, ApiError, BlockTime, ContractPackageHash, Key, RuntimeArgs, URef, U128, U256,
   |                             ^^^^^^^^^
   |
   = note: `#[warn(unused_imports)]` on by default

warning: unused import: `renvm_sig::hash_message`
  --> pair/src/pair.rs:17:5
   |
17 | use renvm_sig::hash_message;
   |     ^^^^^^^^^^^^^^^^^^^^^^^

warning: unused import: `renvm_sig::keccak256`
  --> pair/src/pair.rs:18:5
   |
18 | use renvm_sig::keccak256;
   |     ^^^^^^^^^^^^^^^^^^^^

warning: value assigned to `liquidity` is never read
   --> pair/src/pair.rs:932:17
    |
932 |         let mut liquidity: U256 = 0.into();
    |                 ^^^^^^^^^
    |
    = note: `#[warn(unused_assignments)]` on by default
    = help: maybe it is overwritten before being read?

warning: `pair` (lib) generated 4 warnings
warning: unused import: `hex::encode`
  --> pair/bin/pair_token.rs:18:5
   |
18 | use hex::encode;
   |     ^^^^^^^^^^^
   |
   = note: `#[warn(unused_imports)]` on by default

warning: unused import: `renvm_sig::keccak256`
  --> pair/bin/pair_token.rs:20:5
   |
20 | use renvm_sig::keccak256;
   |     ^^^^^^^^^^^^^^^^^^^^

warning: `pair` (bin "pair-token") generated 2 warnings
    Finished release [optimized] target(s) in 0.49s
wasm-strip target/wasm32-unknown-unknown/release/pair-token.wasm 2>/dev/null | true
make[1]: Leaving directory '/workspace/CasperLabs-UniswapV2-Core/pair'
cd ../CasperLabs-UniswapV2-Core/wcspr/ && make build-contract
make[1]: Entering directory '/workspace/CasperLabs-UniswapV2-Core/wcspr'
cargo build --release -p wcspr --target wasm32-unknown-unknown
warning: profiles for the non root package will be ignored, specify profiles at the workspace root:
package:   /workspace/CasperLabs-UniswapV2-Core/wcspr/test-contract/Cargo.toml
workspace: /workspace/CasperLabs-UniswapV2-Core/wcspr/Cargo.toml
warning: profiles for the non root package will be ignored, specify profiles at the workspace root:
package:   /workspace/CasperLabs-UniswapV2-Core/wcspr/test-contract2/Cargo.toml
workspace: /workspace/CasperLabs-UniswapV2-Core/wcspr/Cargo.toml
warning: Patch `renvm-sig v0.1.1 (https://github.com/Scytalelabs-official/CasperLabs-renvm-sig.git?branch=main#bb97d895)` was not used in the crate graph.
Check that the patched package version and available features are compatible
with the dependency requirements. If the patch has a different version from
what is locked in the Cargo.lock file, run `cargo update` to use the new
version. This may also occur with an optional dependency that is not enabled.
    Finished release [optimized] target(s) in 0.52s
wasm-strip target/wasm32-unknown-unknown/release/wcspr-token.wasm 2>/dev/null | true
make[1]: Leaving directory '/workspace/CasperLabs-UniswapV2-Core/wcspr'
cd ../CasperLabs-UniswapV2-Router/uniswap-v2-library/ && make build-contract
make[1]: Entering directory '/workspace/CasperLabs-UniswapV2-Router/uniswap-v2-library'
cargo build --release -p uniswap-v2-library --target wasm32-unknown-unknown
    Finished release [optimized] target(s) in 0.37s
wasm-strip target/wasm32-unknown-unknown/release/uniswap-v2-library.wasm 2>/dev/null | true
make[1]: Leaving directory '/workspace/CasperLabs-UniswapV2-Router/uniswap-v2-library'
cd ../CasperLabs-UniswapV2-Router/uniswap-v2-router/ && make build-contract
make[1]: Entering directory '/workspace/CasperLabs-UniswapV2-Router/uniswap-v2-router'
cargo build --release -p uniswap-v2-router --target wasm32-unknown-unknown
    Finished release [optimized] target(s) in 0.38s
wasm-strip uniswap-v2-router/target/wasm32-unknown-unknown/release/uniswap-v2-router.wasm 2>/dev/null | true
make[1]: Leaving directory '/workspace/CasperLabs-UniswapV2-Router/uniswap-v2-router'
cd ../CasperLabs-StakeableToken/ && make build-all
make[1]: Entering directory '/workspace/CasperLabs-StakeableToken'
make build-stakeable-token
make[2]: Entering directory '/workspace/CasperLabs-StakeableToken'
cargo build --release -p stakeable-token -p session-code-stakeable --target wasm32-unknown-unknown
warning: patch for the non root package will be ignored, specify patch at the workspace root:
package:   /workspace/CasperLabs-StakeableToken/crates/helper/Cargo.toml
workspace: /workspace/CasperLabs-StakeableToken/Cargo.toml
    Finished release [optimized] target(s) in 0.37s
make[2]: Leaving directory '/workspace/CasperLabs-StakeableToken'
make build-liquidity-guard
make[2]: Entering directory '/workspace/CasperLabs-StakeableToken'
cargo build --release -p liquidity-guard -p session-code-liquidity-guard --target wasm32-unknown-unknown
warning: patch for the non root package will be ignored, specify patch at the workspace root:
package:   /workspace/CasperLabs-StakeableToken/crates/helper/Cargo.toml
workspace: /workspace/CasperLabs-StakeableToken/Cargo.toml
    Finished release [optimized] target(s) in 0.06s
make[2]: Leaving directory '/workspace/CasperLabs-StakeableToken'
make[1]: Leaving directory '/workspace/CasperLabs-StakeableToken'
cd . && make build-contract
make[1]: Entering directory '/workspace/CasperLabs-LiquidityTransformer'
cargo build --release -p liquidity_transformer -p scspr -p session-code-lt -p session-code-scspr --target wasm32-unknown-unknown
warning: patch for the non root package will be ignored, specify patch at the workspace root:
package:   /workspace/CasperLabs-LiquidityTransformer/liquidity_transformer/liquidity_transformer_crate/Cargo.toml
workspace: /workspace/CasperLabs-LiquidityTransformer/Cargo.toml
warning: patch for the non root package will be ignored, specify patch at the workspace root:
package:   /workspace/CasperLabs-LiquidityTransformer/liquidity_transformer/liquidity_transformer_tests/Cargo.toml
workspace: /workspace/CasperLabs-LiquidityTransformer/Cargo.toml
    Finished release [optimized] target(s) in 0.06s
make[1]: Leaving directory '/workspace/CasperLabs-LiquidityTransformer'
make copy-wasm-file
make[1]: Entering directory '/workspace/CasperLabs-LiquidityTransformer'
cp ../CasperLabs-UniswapV2-Core/erc20/target/wasm32-unknown-unknown/release/*.wasm ./liquidity_transformer/liquidity_transformer_tests/wasm/
cp ../CasperLabs-UniswapV2-Core/factory/target/wasm32-unknown-unknown/release/*.wasm ./liquidity_transformer/liquidity_transformer_tests/wasm/
cp ../CasperLabs-UniswapV2-Core/flashswapper/target/wasm32-unknown-unknown/release/*.wasm ./liquidity_transformer/liquidity_transformer_tests/wasm/
cp ../CasperLabs-UniswapV2-Core/pair/target/wasm32-unknown-unknown/release/*.wasm ./liquidity_transformer/liquidity_transformer_tests/wasm/
cp ../CasperLabs-UniswapV2-Core/wcspr/target/wasm32-unknown-unknown/release/*.wasm ./liquidity_transformer/liquidity_transformer_tests/wasm/
cp ../CasperLabs-UniswapV2-Router/uniswap-v2-router/target/wasm32-unknown-unknown/release/*.wasm ./liquidity_transformer/liquidity_transformer_tests/wasm/
cp ../CasperLabs-UniswapV2-Router/uniswap-v2-library/target/wasm32-unknown-unknown/release/*.wasm ./liquidity_transformer/liquidity_transformer_tests/wasm/
cp ../CasperLabs-StakeableToken/target/wasm32-unknown-unknown/release/*.wasm ./liquidity_transformer/liquidity_transformer_tests/wasm/
cp ./target/wasm32-unknown-unknown/release/*.wasm ./liquidity_transformer/liquidity_transformer_tests/wasm/
cp ../CasperLabs-UniswapV2-Core/erc20/target/wasm32-unknown-unknown/release/*.wasm ./scspr/scspr_tests/wasm/
cp ../CasperLabs-UniswapV2-Core/factory/target/wasm32-unknown-unknown/release/*.wasm ./scspr/scspr_tests/wasm/
cp ../CasperLabs-UniswapV2-Core/flashswapper/target/wasm32-unknown-unknown/release/*.wasm ./scspr/scspr_tests/wasm/
cp ../CasperLabs-UniswapV2-Core/pair/target/wasm32-unknown-unknown/release/*.wasm ./scspr/scspr_tests/wasm/
cp ../CasperLabs-UniswapV2-Core/wcspr/target/wasm32-unknown-unknown/release/*.wasm ./scspr/scspr_tests/wasm/
cp ../CasperLabs-UniswapV2-Router/uniswap-v2-router/target/wasm32-unknown-unknown/release/*.wasm ./scspr/scspr_tests/wasm/
cp ../CasperLabs-UniswapV2-Router/uniswap-v2-library/target/wasm32-unknown-unknown/release/*.wasm ./scspr/scspr_tests/wasm/
cp ../CasperLabs-StakeableToken/target/wasm32-unknown-unknown/release/*.wasm ./scspr/scspr_tests/wasm/
cp ./target/wasm32-unknown-unknown/release/*.wasm ./scspr/scspr_tests/wasm/
make[1]: Leaving directory '/workspace/CasperLabs-LiquidityTransformer'
```

## Test Deploys of the Smart Contracts
- [DAI Contract](https://testnet.cspr.live/contract/68e653a5595f3d98d3fa2808a44f74fc038bc3fd47828d11143afd34f4be7b0e)
- [DAI Contract Package](https://testnet.cspr.live/contract-package/40651f7974f55bc40762ac7e0ea79ec956d10dfba0bbc13191e44525267847d0)
- [Factory Contract](https://testnet.cspr.live/contract/93652a1de1f866f26bafb94158b42fe7b19bb350c8277dd7b86e85fa348a3b83)
- [Factory Contract Package](https://testnet.cspr.live/contract-package/7e4561f4259e964c8dc0a69afbef8718008ff0f81a862092b86cfd9fad649486)
- [Flash Swapper Contract](https://testnet.cspr.live/contract/3ab99a72531a791d6c49ef4b62f85bed6b59b65c2d7567fbdfe9bef53c4092d5)
- [Flash Swapper Contract Package](https://testnet.cspr.live/contract-package/d23587f34bed542f3be0562e5fa1a3be846f7ad8c68b472e9bd5b4987c782759)
- [Library Contract](https://testnet.cspr.live/contract/34b7a36d0d8c017a35909832a9bd641d90c66698bffbc9a02f53d796cd344572)
- [Library Contract Package](https://testnet.cspr.live/contract-package/95f0e9a525005fcb0c6f5fec988c33523eb0ff116bea1350e152e3304f1b3af7)
- [Liquidity Guard Contract](https://testnet.cspr.live/contract/a8226e658b31a5dd3885ca670218cda176bf789c1a26e4c1935fbaa6a41213ea)
- [Liquidity Guard Contract Package](https://testnet.cspr.live/contract-package/33433220f3376db18d291866f12a7bd2b593827f434a77e7ec2f6aeec3427b5e)
- [Liquidity Transformer Contract](https://testnet.cspr.live/contract/d5aad3c75eb6dc5da8f23b5af451426a38b66092f21db32ad399a7040852b39d)
- [Liquidity Transformer Contract Package](https://testnet.cspr.live/contract-package/30f187817b03acbd95bed90948297605d1f8be2bb2ccf06bdcd293d8e87c7814)
- [ScsprWcspr Pair Contract](https://testnet.cspr.live/contract/e4d39f7b03188dbdab79fdf6825ff8b9db6106e93a6a381a7bbab43d70db54bf)
- [ScsprWcspr Pair Contract Package](https://testnet.cspr.live/contract-package/d17546e15f80f84e7a4dc0f748179ea8c984a08a6bc0b4a9e6232c0d7e8e09f5)
- [SUSDWcspr Pair Contract](https://testnet.cspr.live/contract/af67e00fdf6589433d5107e466ebdb7086dbde995ba183656081dbb6ae8230a7)
- [SUSDWcspr Pair Contract Package](https://testnet.cspr.live/contract-package/b61c2cf918f6573ad8bf7ef36f0a22b64a7a41bf72f1e6e7e2cdb94d56520b31)
- [WiseScspr Pair Contract](https://testnet.cspr.live/contract/5c94d133fd12e8a3fc366a31a681d7dad1f2f59a95588052fcfac63fb2ed65cb)
- [WiseScspr Pair Contract Package](https://testnet.cspr.live/contract-package/3d0a11016c08dbfe2f7dfe09e0c38b4aac00a55fc381987a16c0a9e468856289)
- [Router Contract](https://testnet.cspr.live/contract/55d52d8ca37507e4d9fdf98ec3e1c9792d863f7b55a4a16b9f301a300888c17f)
- [Router Contract Package](https://testnet.cspr.live/contract-package/d29c4205c011ef975d509a1c663def6fbd70eb6a470a14331ac6ef141dedc630)
- [scspr Contract](https://testnet.cspr.live/contract/c6606a2f6cec50704150e7056d0438924662051cce33fdf25f2311975985a2a0)
- [scspr Contract Package](https://testnet.cspr.live/contract-package/fec79ab37063627f9a7910628edd47c377a9ed3ea70e8355438fdd8231e51ec7)
- [Stable USD Contract](https://testnet.cspr.live/contract/8cf140a8ca8682e22e04c817779d4ec066b92494ed805f34cc0218a6358c0b94)
- [Stable USD Contract Package](https://testnet.cspr.live/contract-package/dfe4c2fa6898d2247984048f392850811b0fb0cafe659e57e18ba5ce19892cc3)
- [Stakeable Contract](https://testnet.cspr.live/contract/bb0a6b948d6c8b75dc265833ad46b2008186573105236e21c52cd98f18da4a21)
- [Stakeable Contract Package](https://testnet.cspr.live/contract-package/c63a157d11c4ea8b50b542b36ffb19a1a5b04fa4395300ff8416dfd4fa4dd9b1)
- [WCSPR Contract](https://testnet.cspr.live/contract/30dd825d4754290eeb1deca390ee7462c3feb069d15d49e9a1c1b207130a4a32)
- [WCSPR Contract Package](https://testnet.cspr.live/contract-package/aa8ba5a4f307c907e6b892d82e8ae39bfdb8a3c35daec51a48eb939be9dccf91)

## Test Runs

```bash
$ make run-all
make run-stakeable-token
make[1]: Entering directory '/workspace/CasperLabs-StakeableToken'
make build-stakeable-token
make[2]: Entering directory '/workspace/CasperLabs-StakeableToken'
cargo build --release -p stakeable-token -p session-code-stakeable --target wasm32-unknown-unknown
warning: patch for the non root package will be ignored, specify patch at the workspace root:
package:   /workspace/CasperLabs-StakeableToken/crates/helper/Cargo.toml
workspace: /workspace/CasperLabs-StakeableToken/Cargo.toml
    Finished release [optimized] target(s) in 0.07s
make[2]: Leaving directory '/workspace/CasperLabs-StakeableToken'
make build-liquidity-guard
make[2]: Entering directory '/workspace/CasperLabs-StakeableToken'
cargo build --release -p liquidity-guard -p session-code-liquidity-guard --target wasm32-unknown-unknown
warning: patch for the non root package will be ignored, specify patch at the workspace root:
package:   /workspace/CasperLabs-StakeableToken/crates/helper/Cargo.toml
workspace: /workspace/CasperLabs-StakeableToken/Cargo.toml
    Finished release [optimized] target(s) in 0.07s
make[2]: Leaving directory '/workspace/CasperLabs-StakeableToken'
make copy-wasm-file-stakeable-token
make[2]: Entering directory '/workspace/CasperLabs-StakeableToken'
cp ../CasperLabs-UniswapV2-Router/uniswap-v2-router/target/wasm32-unknown-unknown/release/uniswap-v2-router.wasm stakeable-token/tests/wasm
cp ../CasperLabs-UniswapV2-Core/factory/target/wasm32-unknown-unknown/release/factory.wasm stakeable-token/tests/wasm
cp ../CasperLabs-UniswapV2-Core/pair/target/wasm32-unknown-unknown/release/pair-token.wasm stakeable-token/tests/wasm
cp ../CasperLabs-UniswapV2-Core/erc20/target/wasm32-unknown-unknown/release/erc20-token.wasm stakeable-token/tests/wasm
cp ../CasperLabs-UniswapV2-Router/uniswap-v2-library/target/wasm32-unknown-unknown/release/uniswap-v2-library.wasm stakeable-token/tests/wasm
cp ../CasperLabs-UniswapV2-Core/wcspr/target/wasm32-unknown-unknown/release/wcspr-token.wasm stakeable-token/tests/wasm
cp ../CasperLabs-UniswapV2-Core/flashswapper/target/wasm32-unknown-unknown/release/flashswapper-token.wasm stakeable-token/tests/wasm
cp ../CasperLabs-LiquidityTransformer/target/wasm32-unknown-unknown/release/scspr.wasm stakeable-token/tests/wasm
cp ../CasperLabs-LiquidityTransformer/target/wasm32-unknown-unknown/release/liquidity_transformer.wasm stakeable-token/tests/wasm
cp ../CasperLabs-LiquidityTransformer/target/wasm32-unknown-unknown/release/session-code-lt.wasm stakeable-token/tests/wasm
cp target/wasm32-unknown-unknown/release/liquidity-guard.wasm stakeable-token/tests/wasm
cp target/wasm32-unknown-unknown/release/stakeable-token.wasm stakeable-token/tests/wasm
cp target/wasm32-unknown-unknown/release/session-code-stakeable.wasm stakeable-token/tests/wasm
make[2]: Leaving directory '/workspace/CasperLabs-StakeableToken'
make test-stakeable-token
make[2]: Entering directory '/workspace/CasperLabs-StakeableToken'
cargo test -p stakeable-token-tests t1
warning: patch for the non root package will be ignored, specify patch at the workspace root:
package:   /workspace/CasperLabs-StakeableToken/crates/helper/Cargo.toml
workspace: /workspace/CasperLabs-StakeableToken/Cargo.toml
    Finished test [unoptimized + debuginfo] target(s) in 0.16s
     Running unittests src/lib.rs (target/debug/deps/stakeable_token_tests-35df09a88d7cc645)

running 2 tests
test tests::t1::should_be_able_to_create_stake_and_end_stake_immature_no_penalty has been running for over 60 seconds
test tests::t1::should_be_able_to_create_stake_with_cspr has been running for over 60 seconds
test tests::t1::should_be_able_to_create_stake_and_end_stake_immature_no_penalty ... ok
test tests::t1::should_be_able_to_create_stake_with_cspr ... ok

test result: ok. 2 passed; 0 failed; 0 ignored; 0 measured; 2 filtered out; finished in 105.11s

cargo test -p stakeable-token-tests t2
warning: patch for the non root package will be ignored, specify patch at the workspace root:
package:   /workspace/CasperLabs-StakeableToken/crates/helper/Cargo.toml
workspace: /workspace/CasperLabs-StakeableToken/Cargo.toml
    Finished test [unoptimized + debuginfo] target(s) in 0.22s
     Running unittests src/lib.rs (target/debug/deps/stakeable_token_tests-35df09a88d7cc645)

running 2 tests
test tests::t2::should_be_able_to_create_stake_and_end_stake_immature_penalty has been running for over 60 seconds
test tests::t2::should_be_able_to_create_stake_and_scrape_interest has been running for over 60 seconds
test tests::t2::should_be_able_to_create_stake_and_scrape_interest ... ok
test tests::t2::should_be_able_to_create_stake_and_end_stake_immature_penalty ... ok

test result: ok. 2 passed; 0 failed; 0 ignored; 0 measured; 2 filtered out; finished in 141.53s

make[2]: Leaving directory '/workspace/CasperLabs-StakeableToken'
make[1]: Leaving directory '/workspace/CasperLabs-StakeableToken'
make run-liquidity-guard
make[1]: Entering directory '/workspace/CasperLabs-StakeableToken'
make build-liquidity-guard
make[2]: Entering directory '/workspace/CasperLabs-StakeableToken'
cargo build --release -p liquidity-guard -p session-code-liquidity-guard --target wasm32-unknown-unknown
warning: patch for the non root package will be ignored, specify patch at the workspace root:
package:   /workspace/CasperLabs-StakeableToken/crates/helper/Cargo.toml
workspace: /workspace/CasperLabs-StakeableToken/Cargo.toml
    Finished release [optimized] target(s) in 0.06s
make[2]: Leaving directory '/workspace/CasperLabs-StakeableToken'
make copy-wasm-file-liquidity-guard
make[2]: Entering directory '/workspace/CasperLabs-StakeableToken'
cp target/wasm32-unknown-unknown/release/liquidity-guard.wasm liquidity-guard/tests/wasm
cp target/wasm32-unknown-unknown/release/session-code-liquidity-guard.wasm liquidity-guard/tests/wasm
make[2]: Leaving directory '/workspace/CasperLabs-StakeableToken'
make test-liquidity-guard
make[2]: Entering directory '/workspace/CasperLabs-StakeableToken'
cargo test -p liquidity-guard-tests
warning: patch for the non root package will be ignored, specify patch at the workspace root:
package:   /workspace/CasperLabs-StakeableToken/crates/helper/Cargo.toml
workspace: /workspace/CasperLabs-StakeableToken/Cargo.toml
    Finished test [unoptimized + debuginfo] target(s) in 0.16s
     Running unittests src/lib.rs (target/debug/deps/liquidity_guard_tests-c5504e092c5b0cf1)

running 2 tests
test tests::get_inflation ... ok
test tests::assign_inflation ... ok

test result: ok. 2 passed; 0 failed; 0 ignored; 0 measured; 0 filtered out; finished in 3.79s

   Doc-tests liquidity-guard-tests

running 0 tests

test result: ok. 0 passed; 0 failed; 0 ignored; 0 measured; 0 filtered out; finished in 0.00s

make[2]: Leaving directory '/workspace/CasperLabs-StakeableToken'
make[1]: Leaving directory '/workspace/CasperLabs-StakeableToken'
```

## Overall Impression of usage testing

It was observed that the project is possible to build and deploy on the TestNet, following the instructions. The test runs and contract calls are also successful. However;
- **The provided deploy script fails due to out-of-gas error when run directly. The reviewer could deploy the smart contracts only after doubling the gas cost amounts set in the script configuration. OP needs to determine the exact costs for each contract, and update the script accordingly, before the final milestone.**
- The provided script does not act well after one of the deploys fails on a previous attempt. It just continues from where it was left, like if the failed deploy was a success, causing more confusing errors later on top of the wasted gas fees. So the reviewer suggests improving the deploy script on that front.
- Although the documentation is generally good in a technical sense, the reviewer suggests providing more coverage, especially focusing on the design decisions, considering the complexity of the project.

Nonetheless, reviewer would like to commend the OP on their hard work to provide a complete script to make it very easy to deploy this giant project on the network.

Overall, the reviewer thinks that this part of the review should PASS with Notes.

Requirement | Finding
------------ | -------------
Project builds without errors | PASS
Documentation provides sufficient installation/execution instructions | PASS with Notes
Project functionality meets/exceeds acceptance criteria and operates without error | PASS

# Unit / Automated Testing

The project has enough coverage with both the positive and the negative paths. However, the tests seem to be heavy on the positive side. So **Reviewer recommends increasing the number of the negative path tests on the project.**

Moreover, not all repositories have CI facilities in place, which is, in Reviewer's opinion, a must-have for a project this size and complexity. Hence, **it is highly recommended to properly setup CI facilities for all repositories which makes sure the code-base of the project is prevented from being subject to software erosion.**

Repository | CI Facilities in Place
------------ | -------------
https://github.com/Rengo-Labs/CasperLabs-StakeableToken | 🔴 No
https://github.com/Rengo-Labs/CasperLabs-LiquidityTransformer | 🔴 No
https://github.com/Rengo-Labs/CasperLabs-UniswapV2-Core | 🟢 Yes
https://github.com/Rengo-Labs/CasperLabs-UniswapV2-Router | 🟡 Broken

## Test Logs
- 

Requirement | Finding
------------ | -------------
Unit Tests - At least one positive path test | PASS
Unit Tests - At least one negative path test | PASS
Unit Tests - Additional path tests | PASS with Notes

# Documentation

### Code Documentation

Project seems to have an acceptable level of code-level documentation for these none-final milestones, considering the proper naming of the functions and the extensive function explanations on the READMEs. However, **Reviewer recommends extending the code-level documentation with proper inline comments which allows auto-generation of code documentation before the final milestone.**

Requirement | Finding
------------ | -------------
Code Documented | PASS with Notes

### Project Documentation

Project documentation is acceptable for this milestone. However, **Reviewer highly suggests the OP to extend the project-level documentation with high-level presentations showing how all pieces of this giant project fit together, to make it maintainable by a future team and/or open-source contributors.** Moreover, Reviewer would like to note that User Documentation requirements of the project need to be revisited during the review of the next milestone which includes the user-level/UI pieces.

Requirement | Finding
------------ | -------------
Usage Documented | PASS with Notes
Example Documented | PASS with Notes


## Overall Conclusion on Documentation

Both the project and the code-level documentation are at an acceptable level for this milestone, but possible improvements are recommended/suggested, as explained by the notes in the earlier sections.

# Open Source Practices

## Licenses

The repository is supposed to be released under the MIT license, as promised on the proposal, but none of the 4 repositories have a MIT license. However, since all of the repositories are licensed under an OSI-approved open-source license, **Reviewer recommends a PASS with Notes for this requirement, provided that the OP updates the licenses on all repositories as MIT before the final milestone**.

Reviewer also would like to note that while all three licenses mentioned in this section are widely used/accepted open-source licenses, there are important differences between them. For one, Apache-2.0 and MIT are both permissive licenses whereas GPL-3.0 is a protective license; and this difference may cause issues for certain projects that would be built upon these code-bases.

Repository | License
------------ | -------------
https://github.com/Rengo-Labs/CasperLabs-StakeableToken | 🟡 Apache-2.0 license
https://github.com/Rengo-Labs/CasperLabs-LiquidityTransformer | 🟡 Apache-2.0 license
https://github.com/Rengo-Labs/CasperLabs-UniswapV2-Core | 🟡 GPL-3.0 license
https://github.com/Rengo-Labs/CasperLabs-UniswapV2-Router | 🟡 GPL-3.0 license

Requirement | Finding
------------ | -------------
OSI-approved open source software license | PASS with Notes

## Contribution Policies

Pull requests and issues are enabled on the repositories. All of the repositories also have security policies and contributing guidelines. However, it was observed that **the contributing policies are in need of a proofread and update to match the realities of their corresponding repositories**. Moreover, the repositories have **no description, website, or topics**, hindering its discoverability.

Although it is not a point of failure, and not part of the requirements of the customer, it was observed that the **Pull/Merge Requests, the de-facto way of contributing to an open-source repository, are hardly used on the project**. Thus, considering the complexity, size, and importance of the project, Reviewer highly suggests the OP's team to adopt the open-source workflow to ensure the sustainability of the project as an open-source code-base.

Repository | Commits | Pull Requests
------------ | ------------- | -------------
https://github.com/Rengo-Labs/CasperLabs-StakeableToken | 48 | 🟡 2
https://github.com/Rengo-Labs/CasperLabs-LiquidityTransformer | 55 | 🔴 0
https://github.com/Rengo-Labs/CasperLabs-UniswapV2-Core | 279 | 🟡 3
https://github.com/Rengo-Labs/CasperLabs-UniswapV2-Router | 22 | 🟡 1

Thus, Reviewer recommends a PASS with Notes on this requirement.

Requirement | Finding
------------ | -------------
OSS contribution best practices | PASS with Notes


# Coding Standards

## General Observations

Code is generally well-structured and readable. The project has been committed to GitHub, has an acceptable level of tests although a bit heavier on the positive paths.

# Final Conclusion

It was observed that the project builds and and runs as expected after small adjustments noted in the previous sections, has successfully running tests, and meets/exceeds the acceptance criteria for the submitted milestones, and adheres to the definition of done provided by the customer.

However, there are certain points that need to be improved/fixed before the final milestone, as well as some non-compulsary recommendations/suggestions, that are expected to be handled by the OP before the final milestone.

Thus, in Reviewer's opinion, this submission should PASS with Notes.

# Recommendation

Recommendation | PASS with Notes
------------ | -------------
