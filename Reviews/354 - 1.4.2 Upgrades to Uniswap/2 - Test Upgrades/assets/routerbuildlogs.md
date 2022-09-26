# Build erc20
cd ../CasperLabs-UniswapV2-Core/erc20/ && make build-contract
make[1]: Entering directory '/workspace/CasperLabs-UniswapV2-Core/erc20'
cargo build --release -p erc20 --target wasm32-unknown-unknown
    Finished release [optimized] target(s) in 0.67s
wasm-strip target/wasm32-unknown-unknown/release/erc20-token.wasm 2>/dev/null | true
make[1]: Leaving directory '/workspace/CasperLabs-UniswapV2-Core/erc20'
# Build factory
cd ../CasperLabs-UniswapV2-Core/factory/ && make build-contract
make[1]: Entering directory '/workspace/CasperLabs-UniswapV2-Core/factory'
cargo build --release -p factory --target wasm32-unknown-unknown
    Finished release [optimized] target(s) in 0.46s
wasm-strip target/wasm32-unknown-unknown/release/factory.wasm 2>/dev/null | true
make[1]: Leaving directory '/workspace/CasperLabs-UniswapV2-Core/factory'
# Build flash swapper
cd ../CasperLabs-UniswapV2-Core/flashswapper/ && make build-contract
make[1]: Entering directory '/workspace/CasperLabs-UniswapV2-Core/flashswapper'
cargo build --release -p flashswapper --target wasm32-unknown-unknown
    Finished release [optimized] target(s) in 0.44s
wasm-strip target/wasm32-unknown-unknown/release/flashswapper-token.wasm 2>/dev/null | true
make[1]: Leaving directory '/workspace/CasperLabs-UniswapV2-Core/flashswapper'
# Build pair
cd ../CasperLabs-UniswapV2-Core/pair/ && make build-contract
make[1]: Entering directory '/workspace/CasperLabs-UniswapV2-Core/pair'
cargo build --release -p pair --target wasm32-unknown-unknown
warning: value assigned to `liquidity` is never read
    --> pair/src/pair.rs:1005:17
     |
1005 |         let mut liquidity: U256 = 0.into();
     |                 ^^^^^^^^^
     |
     = note: `#[warn(unused_assignments)]` on by default
     = help: maybe it is overwritten before being read?

warning: `pair` (lib) generated 1 warning
    Finished release [optimized] target(s) in 0.48s
wasm-strip target/wasm32-unknown-unknown/release/pair-token.wasm 2>/dev/null | true
make[1]: Leaving directory '/workspace/CasperLabs-UniswapV2-Core/pair'
# Build wcspr
cd ../CasperLabs-UniswapV2-Core/wcspr/ && make build-contract
make[1]: Entering directory '/workspace/CasperLabs-UniswapV2-Core/wcspr'
cargo build --release -p wcspr --target wasm32-unknown-unknown
warning: profiles for the non root package will be ignored, specify profiles at the workspace root:
package:   /workspace/CasperLabs-UniswapV2-Core/wcspr/test-contract/Cargo.toml
workspace: /workspace/CasperLabs-UniswapV2-Core/wcspr/Cargo.toml
warning: profiles for the non root package will be ignored, specify profiles at the workspace root:
package:   /workspace/CasperLabs-UniswapV2-Core/wcspr/test-contract2/Cargo.toml
workspace: /workspace/CasperLabs-UniswapV2-Core/wcspr/Cargo.toml
    Finished release [optimized] target(s) in 0.46s
wasm-strip target/wasm32-unknown-unknown/release/wcspr-token.wasm 2>/dev/null | true
make[1]: Leaving directory '/workspace/CasperLabs-UniswapV2-Core/wcspr'
# Build Library
cd ./uniswap-v2-library/ && make build-contract
make[1]: Entering directory '/workspace/CasperLabs-UniswapV2-Router/uniswap-v2-library'
cargo build --release -p uniswap-v2-library --target wasm32-unknown-unknown
    Finished release [optimized] target(s) in 0.47s
wasm-strip target/wasm32-unknown-unknown/release/uniswap-v2-library.wasm 2>/dev/null | true
make[1]: Leaving directory '/workspace/CasperLabs-UniswapV2-Router/uniswap-v2-library'
# Build Router
cd ./uniswap-v2-router/ && make build-contract
make[1]: Entering directory '/workspace/CasperLabs-UniswapV2-Router/uniswap-v2-router'
cargo build --release -p uniswap-v2-router --target wasm32-unknown-unknown
    Finished release [optimized] target(s) in 0.49s
wasm-strip uniswap-v2-router/target/wasm32-unknown-unknown/release/uniswap-v2-router.wasm 2>/dev/null | true
make[1]: Leaving directory '/workspace/CasperLabs-UniswapV2-Router/uniswap-v2-router'
# Build Test_Contract
cd ./uniswap-v2-router-test-contract/test-contract/ && cargo build --release
    Finished release [optimized] target(s) in 0.43s
# copy wasm files
make copy-wasm-file
make[1]: Entering directory '/workspace/CasperLabs-UniswapV2-Router'
cp ../CasperLabs-UniswapV2-Core/erc20/target/wasm32-unknown-unknown/release/*.wasm ./uniswap-v2-library//uniswap-v2-library-tests/wasm/
cp ../CasperLabs-UniswapV2-Core/factory/target/wasm32-unknown-unknown/release/*.wasm ./uniswap-v2-library//uniswap-v2-library-tests/wasm/
cp ../CasperLabs-UniswapV2-Core/flashswapper/target/wasm32-unknown-unknown/release/*.wasm ./uniswap-v2-library//uniswap-v2-library-tests/wasm/
cp ../CasperLabs-UniswapV2-Core/pair/target/wasm32-unknown-unknown/release/*.wasm ./uniswap-v2-library//uniswap-v2-library-tests/wasm/
cp ../CasperLabs-UniswapV2-Core/wcspr/target/wasm32-unknown-unknown/release/*.wasm ./uniswap-v2-library//uniswap-v2-library-tests/wasm/
cp ./uniswap-v2-router/target/wasm32-unknown-unknown/release/*.wasm ./uniswap-v2-library//uniswap-v2-library-tests/wasm/
cp ./uniswap-v2-router-test-contract/test-contract/target/wasm32-unknown-unknown/release/*.wasm ./uniswap-v2-library//uniswap-v2-library-tests/wasm/
cp ../CasperLabs-UniswapV2-Core/erc20/target/wasm32-unknown-unknown/release/*.wasm ./uniswap-v2-router//uniswap-v2-router-tests/wasm/
cp ../CasperLabs-UniswapV2-Core/factory/target/wasm32-unknown-unknown/release/*.wasm ./uniswap-v2-router//uniswap-v2-router-tests/wasm/
cp ../CasperLabs-UniswapV2-Core/flashswapper/target/wasm32-unknown-unknown/release/*.wasm ./uniswap-v2-router//uniswap-v2-router-tests/wasm/
cp ../CasperLabs-UniswapV2-Core/pair/target/wasm32-unknown-unknown/release/*.wasm ./uniswap-v2-router//uniswap-v2-router-tests/wasm/
cp ../CasperLabs-UniswapV2-Core/wcspr/target/wasm32-unknown-unknown/release/*.wasm ./uniswap-v2-router//uniswap-v2-router-tests/wasm/
cp ./uniswap-v2-library/target/wasm32-unknown-unknown/release/*.wasm ./uniswap-v2-router//uniswap-v2-router-tests/wasm/
cp ./uniswap-v2-router-test-contract/test-contract/target/wasm32-unknown-unknown/release/*.wasm ./uniswap-v2-router//uniswap-v2-router-tests/wasm/
make[1]: Leaving directory '/workspace/CasperLabs-UniswapV2-Router'
