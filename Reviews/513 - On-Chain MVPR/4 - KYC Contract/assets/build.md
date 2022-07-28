oc@foc:~/dao-contracts$ make build-all
cargo build --release --target wasm32-unknown-unknown --quiet --features=wasm --no-default-features -p casper-dao-contracts
info: syncing channel updates for 'nightly-2021-06-17-x86_64-unknown-linux-gnu'
info: latest update on 2021-06-17, rust version 1.55.0-nightly (a85f584ae 2021-06-16)
info: downloading component 'cargo'
info: downloading component 'clippy'
info: downloading component 'rust-docs'
info: downloading component 'rust-std'
info: downloading component 'rustc'
info: downloading component 'rustfmt'
info: installing component 'cargo'
info: installing component 'clippy'
info: installing component 'rust-docs'
info: installing component 'rust-std'
info: installing component 'rustc'
info: installing component 'rustfmt'
error[E0463]: can't find crate for `core`
  |
  = note: the `wasm32-unknown-unknown` target may not be installed
  = help: consider downloading the target with `rustup target add wasm32-unknown-unknown`
  = help: consider building the standard library from source with `cargo build -Zbuild-std`

error: aborting due to previous error

For more information about this error, try `rustc --explain E0463`.
error: could not compile `subtle`

To learn more, run the command again with --verbose.
error: build failed
make: *** [Makefile:14: build-dao-contracts] Error 101
foc@foc:~/dao-contracts$ rustup target add wasm32-unknown-unknown
info: downloading component 'rust-std' for 'wasm32-unknown-unknown'
info: installing component 'rust-std' for 'wasm32-unknown-unknown'
 13.4 MiB /  13.4 MiB (100 %)  13.0 MiB/s in  1s ETA:  0s
foc@foc:~/dao-contracts$ make build-all
cargo build --release --target wasm32-unknown-unknown --quiet --features=wasm --no-default-features -p casper-dao-contracts
cargo build --release --target wasm32-unknown-unknown --quiet --features=wasm --no-default-features -p casper-dao-erc20
cargo build --release --target wasm32-unknown-unknown --quiet --features=wasm --no-default-features -p casper-dao-erc721
