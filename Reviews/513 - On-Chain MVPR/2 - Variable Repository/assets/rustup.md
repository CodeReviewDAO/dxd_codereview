```
@ggurbet ➜ /workspaces/dao-contracts (7c24f46) $ curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh
info: downloading installer

Welcome to Rust!

This will download and install the official compiler for the Rust
programming language, and its package manager, Cargo.

Rustup metadata and toolchains will be installed into the Rustup
home directory, located at:

  /home/codespace/.rustup

This can be modified with the RUSTUP_HOME environment variable.

The Cargo home directory is located at:

  /home/codespace/.cargo

This can be modified with the CARGO_HOME environment variable.

The cargo, rustc, rustup and other commands will be added to
Cargo's bin directory, located at:

  /home/codespace/.cargo/bin

This path will then be added to your PATH environment variable by
modifying the profile files located at:

  /home/codespace/.profile
  /home/codespace/.bashrc
  /home/codespace/.zshenv

You can uninstall at any time with rustup self uninstall and
these changes will be reverted.

Current installation options:


   default host triple: x86_64-unknown-linux-gnu
     default toolchain: stable (default)
               profile: default
  modify PATH variable: yes

1) Proceed with installation (default)
2) Customize installation
3) Cancel installation
>1

info: profile set to 'default'
info: default host triple is x86_64-unknown-linux-gnu
info: syncing channel updates for 'stable-x86_64-unknown-linux-gnu'
info: latest update on 2022-06-30, rust version 1.62.0 (a8314ef7d 2022-06-27)
info: downloading component 'cargo'
info: downloading component 'clippy'
info: downloading component 'rust-docs'
info: downloading component 'rust-std'
info: downloading component 'rustc'
info: downloading component 'rustfmt'
info: installing component 'cargo'
info: installing component 'clippy'
info: installing component 'rust-docs'
 18.3 MiB /  18.3 MiB (100 %)   6.2 MiB/s in  2s ETA:  0s
info: installing component 'rust-std'
 26.0 MiB /  26.0 MiB (100 %)  11.6 MiB/s in  4s ETA:  0s
info: installing component 'rustc'
 54.1 MiB /  54.1 MiB (100 %)  12.6 MiB/s in  4s ETA:  0s
info: installing component 'rustfmt'
info: default toolchain set to 'stable-x86_64-unknown-linux-gnu'

  stable-x86_64-unknown-linux-gnu installed - rustc 1.62.0 (a8314ef7d 2022-06-27)


Rust is installed now. Great!

To get started you may need to restart your current shell.
This would reload your PATH environment variable to include
Cargo's bin directory ($HOME/.cargo/bin).

To configure your current shell, run:
source "$HOME/.cargo/env"

@ggurbet ➜ /workspaces/dao-contracts (7c24f46) $ source "$HOME/.cargo/env"
@ggurbet ➜ /workspaces/dao-contracts (7c24f46) $ rustc --version
rustc 1.55.0-nightly (a85f584ae 2021-06-16)
@ggurbet ➜ /workspaces/dao-contracts (7c24f46) $ rustup --version
rustup 1.25.1 (bb60b1e89 2022-07-12)
info: This is the version for the rustup toolchain manager, not the rustc compiler.
info: The currently active `rustc` version is `rustc 1.55.0-nightly (a85f584ae 2021-06-16)`
@ggurbet ➜ /workspaces/dao-contracts (7c24f46) $ cargo --version
cargo 1.54.0-nightly (44456677b 2021-06-12)
```