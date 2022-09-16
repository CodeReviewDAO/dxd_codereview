# Build erc20
cd ./erc20/ && make prepare && make build-contract && make build-proxy-contract
make[1]: Entering directory '/workspace/CasperLabs-UniswapV2-Core/erc20'
rustup target add wasm32-unknown-unknown
info: component 'rust-std' for target 'wasm32-unknown-unknown' is up to date
make[1]: Leaving directory '/workspace/CasperLabs-UniswapV2-Core/erc20'
make[1]: Entering directory '/workspace/CasperLabs-UniswapV2-Core/erc20'
cargo build --release -p erc20 --target wasm32-unknown-unknown
    Finished release [optimized] target(s) in 0.05s
wasm-strip target/wasm32-unknown-unknown/release/erc20-token.wasm 2>/dev/null | true
make[1]: Leaving directory '/workspace/CasperLabs-UniswapV2-Core/erc20'
make[1]: Entering directory '/workspace/CasperLabs-UniswapV2-Core/erc20'
cargo build --release -p erc20-proxy --target wasm32-unknown-unknown
    Finished release [optimized] target(s) in 0.05s
wasm-strip target/wasm32-unknown-unknown/release/erc20-proxy-token.wasm 2>/dev/null | true
make[1]: Leaving directory '/workspace/CasperLabs-UniswapV2-Core/erc20'
# Build wcspr
cd ./wcspr/ && make prepare && make build-contract && make build-test-contract && make build-test-contract2
make[1]: Entering directory '/workspace/CasperLabs-UniswapV2-Core/wcspr'
rustup target add wasm32-unknown-unknown
info: component 'rust-std' for target 'wasm32-unknown-unknown' is up to date
make[1]: Leaving directory '/workspace/CasperLabs-UniswapV2-Core/wcspr'
make[1]: Entering directory '/workspace/CasperLabs-UniswapV2-Core/wcspr'
cargo build --release -p wcspr --target wasm32-unknown-unknown
warning: profiles for the non root package will be ignored, specify profiles at the workspace root:
package:   /workspace/CasperLabs-UniswapV2-Core/wcspr/test-contract/Cargo.toml
workspace: /workspace/CasperLabs-UniswapV2-Core/wcspr/Cargo.toml
warning: profiles for the non root package will be ignored, specify profiles at the workspace root:
package:   /workspace/CasperLabs-UniswapV2-Core/wcspr/test-contract2/Cargo.toml
workspace: /workspace/CasperLabs-UniswapV2-Core/wcspr/Cargo.toml
    Finished release [optimized] target(s) in 0.05s
wasm-strip target/wasm32-unknown-unknown/release/wcspr-token.wasm 2>/dev/null | true
make[1]: Leaving directory '/workspace/CasperLabs-UniswapV2-Core/wcspr'
make[1]: Entering directory '/workspace/CasperLabs-UniswapV2-Core/wcspr'
cargo build --release -p test --target wasm32-unknown-unknown
warning: profiles for the non root package will be ignored, specify profiles at the workspace root:
package:   /workspace/CasperLabs-UniswapV2-Core/wcspr/test-contract/Cargo.toml
workspace: /workspace/CasperLabs-UniswapV2-Core/wcspr/Cargo.toml
warning: profiles for the non root package will be ignored, specify profiles at the workspace root:
package:   /workspace/CasperLabs-UniswapV2-Core/wcspr/test-contract2/Cargo.toml
workspace: /workspace/CasperLabs-UniswapV2-Core/wcspr/Cargo.toml
    Finished release [optimized] target(s) in 0.04s
wasm-strip target/wasm32-unknown-unknown/release/wcspr-test.wasm 2>/dev/null | true
make[1]: Leaving directory '/workspace/CasperLabs-UniswapV2-Core/wcspr'
make[1]: Entering directory '/workspace/CasperLabs-UniswapV2-Core/wcspr'
cargo build --release -p test2 --target wasm32-unknown-unknown
warning: profiles for the non root package will be ignored, specify profiles at the workspace root:
package:   /workspace/CasperLabs-UniswapV2-Core/wcspr/test-contract/Cargo.toml
workspace: /workspace/CasperLabs-UniswapV2-Core/wcspr/Cargo.toml
warning: profiles for the non root package will be ignored, specify profiles at the workspace root:
package:   /workspace/CasperLabs-UniswapV2-Core/wcspr/test-contract2/Cargo.toml
workspace: /workspace/CasperLabs-UniswapV2-Core/wcspr/Cargo.toml
    Finished release [optimized] target(s) in 0.04s
wasm-strip target/wasm32-unknown-unknown/release/wcspr-test2.wasm 2>/dev/null | true
make[1]: Leaving directory '/workspace/CasperLabs-UniswapV2-Core/wcspr'
# Build factory
cd ./factory/ && make prepare && make build-contract
make[1]: Entering directory '/workspace/CasperLabs-UniswapV2-Core/factory'
rustup target add wasm32-unknown-unknown
info: component 'rust-std' for target 'wasm32-unknown-unknown' is up to date
make[1]: Leaving directory '/workspace/CasperLabs-UniswapV2-Core/factory'
make[1]: Entering directory '/workspace/CasperLabs-UniswapV2-Core/factory'
cargo build --release -p factory --target wasm32-unknown-unknown
    Finished release [optimized] target(s) in 0.05s
wasm-strip target/wasm32-unknown-unknown/release/factory.wasm 2>/dev/null | true
make[1]: Leaving directory '/workspace/CasperLabs-UniswapV2-Core/factory'
# Build flash swapper
cd ./flashswapper/ && make prepare && make build-contract
make[1]: Entering directory '/workspace/CasperLabs-UniswapV2-Core/flashswapper'
rustup target add wasm32-unknown-unknown
info: component 'rust-std' for target 'wasm32-unknown-unknown' is up to date
make[1]: Leaving directory '/workspace/CasperLabs-UniswapV2-Core/flashswapper'
make[1]: Entering directory '/workspace/CasperLabs-UniswapV2-Core/flashswapper'
cargo build --release -p flashswapper --target wasm32-unknown-unknown
    Finished release [optimized] target(s) in 0.06s
wasm-strip target/wasm32-unknown-unknown/release/flashswapper-token.wasm 2>/dev/null | true
make[1]: Leaving directory '/workspace/CasperLabs-UniswapV2-Core/flashswapper'
# Build pair
cd ./pair/ && make prepare && make build-contract && make build-test-contract && make build-test-contract2
make[1]: Entering directory '/workspace/CasperLabs-UniswapV2-Core/pair'
rustup target add wasm32-unknown-unknown
info: component 'rust-std' for target 'wasm32-unknown-unknown' is up to date
make[1]: Leaving directory '/workspace/CasperLabs-UniswapV2-Core/pair'
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
    Finished release [optimized] target(s) in 0.06s
wasm-strip target/wasm32-unknown-unknown/release/pair-token.wasm 2>/dev/null | true
make[1]: Leaving directory '/workspace/CasperLabs-UniswapV2-Core/pair'
make[1]: Entering directory '/workspace/CasperLabs-UniswapV2-Core/pair'
cargo build --release -p test --target wasm32-unknown-unknown
    Finished release [optimized] target(s) in 0.05s
wasm-strip target/wasm32-unknown-unknown/release/pair-test.wasm 2>/dev/null | true
make[1]: Leaving directory '/workspace/CasperLabs-UniswapV2-Core/pair'
make[1]: Entering directory '/workspace/CasperLabs-UniswapV2-Core/pair'
cargo build --release -p test2 --target wasm32-unknown-unknown
    Finished release [optimized] target(s) in 0.05s
wasm-strip target/wasm32-unknown-unknown/release/pair-test2.wasm 2>/dev/null | true
make[1]: Leaving directory '/workspace/CasperLabs-UniswapV2-Core/pair'
# copy wasm files
make copy-wasm-file
make[1]: Entering directory '/workspace/CasperLabs-UniswapV2-Core'
cp ./erc20/target/wasm32-unknown-unknown/release/*.wasm ./factory/factory-tests/wasm/
cp ./erc20/target/wasm32-unknown-unknown/release/*.wasm ./flashswapper/flashswapper-tests/wasm/
cp ./erc20/target/wasm32-unknown-unknown/release/*.wasm ./pair/pair-tests/wasm/
cp ./wcspr/target/wasm32-unknown-unknown/release/*.wasm ./factory/factory-tests/wasm/
cp ./wcspr/target/wasm32-unknown-unknown/release/*.wasm ./flashswapper/flashswapper-tests/wasm/
cp ./wcspr/target/wasm32-unknown-unknown/release/*.wasm ./pair/pair-tests/wasm/
cp ./pair/target/wasm32-unknown-unknown/release/*.wasm ./factory/factory-tests/wasm/
cp ./pair/target/wasm32-unknown-unknown/release/*.wasm ./flashswapper/flashswapper-tests/wasm/
cp ./flashswapper/target/wasm32-unknown-unknown/release/*.wasm ./factory/factory-tests/wasm/
cp ./flashswapper/target/wasm32-unknown-unknown/release/*.wasm ./pair/pair-tests/wasm/
cp ./factory/target/wasm32-unknown-unknown/release/*.wasm ./flashswapper/flashswapper-tests/wasm/
cp ./factory/target/wasm32-unknown-unknown/release/*.wasm ./pair/pair-tests/wasm/
make[1]: Leaving directory '/workspace/CasperLabs-UniswapV2-Core'
