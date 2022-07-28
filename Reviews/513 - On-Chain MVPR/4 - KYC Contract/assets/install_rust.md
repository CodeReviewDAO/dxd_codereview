foc@foc:~/dao-contracts$ curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh
info: downloading installer
warning: it looks like you have an existing installation of Rust at:
warning: /usr/bin
warning: rustup should not be installed alongside Rust. Please uninstall your existing Rust first.
warning: Otherwise you may have confusion unless you are careful with your PATH
warning: If you are sure that you want both rustup and your already installed Rust
warning: then please reply `y' or `yes' or set RUSTUP_INIT_SKIP_PATH_CHECK to yes
warning: or pass `-y' to ignore all ignorable checks.
error: cannot install while Rust is installed

Continue? (y/N) y


Welcome to Rust!

This will download and install the official compiler for the Rust
programming language, and its package manager, Cargo.

Rustup metadata and toolchains will be installed into the Rustup
home directory, located at:

  /home/foc/.rustup

This can be modified with the RUSTUP_HOME environment variable.

The Cargo home directory is located at:

  /home/foc/.cargo

This can be modified with the CARGO_HOME environment variable.

The cargo, rustc, rustup and other commands will be added to
Cargo's bin directory, located at:

  /home/foc/.cargo/bin

This path will then be added to your PATH environment variable by
modifying the profile files located at:

  /home/foc/.profile
  /home/foc/.bashrc

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
warning: Updating existing toolchain, profile choice will be ignored
info: syncing channel updates for 'stable-x86_64-unknown-linux-gnu'
info: latest update on 2022-07-19, rust version 1.62.1 (e092d0b6b 2022-07-16)
info: downloading component 'cargo'
  6.6 MiB /   6.6 MiB (100 %)   3.2 MiB/s in  2s ETA:  0s
info: downloading component 'clippy'
  2.7 MiB /   2.7 MiB (100 %)   2.0 MiB/s in  1s ETA:  0s
info: downloading component 'rust-docs'
 18.3 MiB /  18.3 MiB (100 %)   1.8 MiB/s in 10s ETA:  0s
info: downloading component 'rust-std'
 26.1 MiB /  26.1 MiB (100 %)   1.8 MiB/s in 14s ETA:  0s
info: downloading component 'rustc'
 54.0 MiB /  54.0 MiB (100 %)   1.8 MiB/s in 29s ETA:  0s
info: downloading component 'rustfmt'
  4.1 MiB /   4.1 MiB (100 %)   2.0 MiB/s in  2s ETA:  0s
info: removing previous version of component 'cargo'
info: removing previous version of component 'clippy'
info: removing previous version of component 'rust-docs'
info: removing previous version of component 'rust-std'
info: removing previous version of component 'rustc'
info: removing previous version of component 'rustfmt'
info: installing component 'cargo'
info: installing component 'clippy'
info: installing component 'rust-docs'
 18.3 MiB /  18.3 MiB (100 %)   6.1 MiB/s in  2s ETA:  0s
info: installing component 'rust-std'
 26.1 MiB /  26.1 MiB (100 %)  12.9 MiB/s in  2s ETA:  0s
info: installing component 'rustc'
 54.0 MiB /  54.0 MiB (100 %)  16.1 MiB/s in  3s ETA:  0s
info: installing component 'rustfmt'
info: default toolchain set to 'stable-x86_64-unknown-linux-gnu'

  stable-x86_64-unknown-linux-gnu updated - rustc 1.62.1 (e092d0b6b 2022-07-16) (from rustc 1.62.0 (a8314ef7d 2022-06-27))


Rust is installed now. Great!

To get started you may need to restart your current shell.
This would reload your PATH environment variable to include
Cargo's bin directory ($HOME/.cargo/bin).

To configure your current shell, run:
source "$HOME/.cargo/env"
