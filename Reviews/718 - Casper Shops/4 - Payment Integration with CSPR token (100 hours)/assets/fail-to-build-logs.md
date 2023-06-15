ndpc_contract (main)$ make build-contract
cd contract && cargo build --release --target wasm32-unknown-unknown
   Compiling typenum v1.15.0
   Compiling autocfg v1.1.0
   Compiling version_check v0.9.4
   Compiling proc-macro2 v1.0.47
   Compiling unicode-ident v1.0.5
   Compiling quote v1.0.21
   Compiling syn v1.0.104
   Compiling rand_core v0.5.1
error[E0463]: can't find crate for `core`
  |
  = note: the `wasm32-unknown-unknown` target may not be installed
  = help: consider downloading the target with `rustup target add wasm32-unknown-unknown`
  = help: consider building the standard library from source with `cargo build -Zbuild-std`

error[E0463]: can't find crate for `compiler_builtins`

error[E0463]: can't find crate for `core`
  --> /home/mehmet/.cargo/registry/src/github.com-1ecc6299db9ec823/rand_core-0.5.1/src/lib.rs:43:5
   |
43 | use core::default::Default;
   |     ^^^^ can't find crate
   |
   = note: the `wasm32-unknown-unknown` target may not be installed
   = help: consider downloading the target with `rustup target add wasm32-unknown-unknown`
   = help: consider building the standard library from source with `cargo build -Zbuild-std`

error[E0463]: can't find crate for `core`
  --> /home/mehmet/.cargo/registry/src/github.com-1ecc6299db9ec823/rand_core-0.5.1/src/lib.rs:44:5
   |
44 | use core::convert::AsMut;
   |     ^^^^ can't find crate
   |
   = note: the `wasm32-unknown-unknown` target may not be installed
   = help: consider downloading the target with `rustup target add wasm32-unknown-unknown`
   = help: consider building the standard library from source with `cargo build -Zbuild-std`

error[E0463]: can't find crate for `core`
  --> /home/mehmet/.cargo/registry/src/github.com-1ecc6299db9ec823/rand_core-0.5.1/src/lib.rs:45:5
   |
45 | use core::ptr::copy_nonoverlapping;
   |     ^^^^ can't find crate
   |
   = note: the `wasm32-unknown-unknown` target may not be installed
   = help: consider downloading the target with `rustup target add wasm32-unknown-unknown`
   = help: consider building the standard library from source with `cargo build -Zbuild-std`

error[E0463]: can't find crate for `core`
  --> /home/mehmet/.cargo/registry/src/github.com-1ecc6299db9ec823/rand_core-0.5.1/src/error.rs:11:5
   |
11 | use core::fmt;
   |     ^^^^ can't find crate
   |
   = note: the `wasm32-unknown-unknown` target may not be installed
   = help: consider downloading the target with `rustup target add wasm32-unknown-unknown`
   = help: consider building the standard library from source with `cargo build -Zbuild-std`

error[E0463]: can't find crate for `core`
  --> /home/mehmet/.cargo/registry/src/github.com-1ecc6299db9ec823/rand_core-0.5.1/src/error.rs:12:5
   |
12 | use core::num::NonZeroU32;
   |     ^^^^ can't find crate
   |
   = note: the `wasm32-unknown-unknown` target may not be installed
   = help: consider downloading the target with `rustup target add wasm32-unknown-unknown`
   = help: consider building the standard library from source with `cargo build -Zbuild-std`

error[E0463]: can't find crate for `core`
  --> /home/mehmet/.cargo/registry/src/github.com-1ecc6299db9ec823/rand_core-0.5.1/src/impls.rs:20:5
   |
20 | use core::ptr::copy_nonoverlapping;
   |     ^^^^ can't find crate
   |
   = note: the `wasm32-unknown-unknown` target may not be installed
   = help: consider downloading the target with `rustup target add wasm32-unknown-unknown`
   = help: consider building the standard library from source with `cargo build -Zbuild-std`

error[E0463]: can't find crate for `core`
  --> /home/mehmet/.cargo/registry/src/github.com-1ecc6299db9ec823/rand_core-0.5.1/src/impls.rs:21:5
   |
21 | use core::slice;
   |     ^^^^ can't find crate
   |
   = note: the `wasm32-unknown-unknown` target may not be installed
   = help: consider downloading the target with `rustup target add wasm32-unknown-unknown`
   = help: consider building the standard library from source with `cargo build -Zbuild-std`

error[E0463]: can't find crate for `core`
  --> /home/mehmet/.cargo/registry/src/github.com-1ecc6299db9ec823/rand_core-0.5.1/src/impls.rs:22:5
   |
22 | use core::cmp::min;
   |     ^^^^ can't find crate
   |
   = note: the `wasm32-unknown-unknown` target may not be installed
   = help: consider downloading the target with `rustup target add wasm32-unknown-unknown`
   = help: consider building the standard library from source with `cargo build -Zbuild-std`

error[E0463]: can't find crate for `core`
  --> /home/mehmet/.cargo/registry/src/github.com-1ecc6299db9ec823/rand_core-0.5.1/src/impls.rs:23:5
   |
23 | use core::mem::size_of;
   |     ^^^^ can't find crate
   |
   = note: the `wasm32-unknown-unknown` target may not be installed
   = help: consider downloading the target with `rustup target add wasm32-unknown-unknown`
   = help: consider building the standard library from source with `cargo build -Zbuild-std`

error[E0463]: can't find crate for `core`
  --> /home/mehmet/.cargo/registry/src/github.com-1ecc6299db9ec823/rand_core-0.5.1/src/block.rs:53:5
   |
53 | use core::convert::AsRef;
   |     ^^^^ can't find crate
   |
   = note: the `wasm32-unknown-unknown` target may not be installed
   = help: consider downloading the target with `rustup target add wasm32-unknown-unknown`
   = help: consider building the standard library from source with `cargo build -Zbuild-std`

error[E0463]: can't find crate for `core`
  --> /home/mehmet/.cargo/registry/src/github.com-1ecc6299db9ec823/rand_core-0.5.1/src/block.rs:54:5
   |
54 | use core::{fmt, ptr};
   |     ^^^^ can't find crate
   |
   = note: the `wasm32-unknown-unknown` target may not be installed
   = help: consider downloading the target with `rustup target add wasm32-unknown-unknown`
   = help: consider building the standard library from source with `cargo build -Zbuild-std`

error[E0463]: can't find crate for `core`
  --> /home/mehmet/.cargo/registry/src/github.com-1ecc6299db9ec823/rand_core-0.5.1/src/le.rs:14:5
   |
14 | use core::ptr;
   |     ^^^^ can't find crate
   |
   = note: the `wasm32-unknown-unknown` target may not be installed
   = help: consider downloading the target with `rustup target add wasm32-unknown-unknown`
   = help: consider building the standard library from source with `cargo build -Zbuild-std`

error: cannot find macro `write` in this scope
   --> /home/mehmet/.cargo/registry/src/github.com-1ecc6299db9ec823/rand_core-0.5.1/src/error.rs:114:13
    |
114 |             write!(f, "Error {{ code: {} }}", self.code)
    |             ^^^^^

error: cannot find macro `write` in this scope
   --> /home/mehmet/.cargo/registry/src/github.com-1ecc6299db9ec823/rand_core-0.5.1/src/error.rs:128:13
    |
128 |             write!(f, "error code {}", self.code)
    |             ^^^^^

error: cannot find macro `cfg` in this scope
   --> /home/mehmet/.cargo/registry/src/github.com-1ecc6299db9ec823/rand_core-0.5.1/src/impls.rs:77:12
    |
77  |         if cfg!(target_endian="little") {
    |            ^^^
...
131 |     fill_via_chunks!(src, dest, u32, 4)
    |     ----------------------------------- in this macro invocation
    |
    = note: `cfg` is in scope, but it is an attribute: `#[cfg]`
    = note: this error originates in the macro `fill_via_chunks` (in Nightly builds, run with -Z macro-backtrace for more info)

error: cannot find macro `cfg` in this scope
   --> /home/mehmet/.cargo/registry/src/github.com-1ecc6299db9ec823/rand_core-0.5.1/src/impls.rs:77:12
    |
77  |         if cfg!(target_endian="little") {
    |            ^^^
...
145 |     fill_via_chunks!(src, dest, u64, 8)
    |     ----------------------------------- in this macro invocation
    |
    = note: `cfg` is in scope, but it is an attribute: `#[cfg]`
    = note: this error originates in the macro `fill_via_chunks` (in Nightly builds, run with -Z macro-backtrace for more info)

error: cannot find attribute `derive` in this scope
   --> /home/mehmet/.cargo/registry/src/github.com-1ecc6299db9ec823/rand_core-0.5.1/src/block.rs:112:3
    |
112 | #[derive(Clone)]
    |   ^^^^^^

error: cannot find macro `assert` in this scope
   --> /home/mehmet/.cargo/registry/src/github.com-1ecc6299db9ec823/rand_core-0.5.1/src/block.rs:166:9
    |
166 |         assert!(index < self.results.as_ref().len());
    |         ^^^^^^

error: cannot find macro `cfg` in this scope
   --> /home/mehmet/.cargo/registry/src/github.com-1ecc6299db9ec823/rand_core-0.5.1/src/block.rs:189:16
    |
189 |             if cfg!(any(target_endian = "little")) {
    |                ^^^
    |
    = note: `cfg` is in scope, but it is an attribute: `#[cfg]`

error: cannot find attribute `derive` in this scope
   --> /home/mehmet/.cargo/registry/src/github.com-1ecc6299db9ec823/rand_core-0.5.1/src/block.rs:285:3
    |
285 | #[derive(Clone)]
    |   ^^^^^^

error: cannot find macro `assert` in this scope
   --> /home/mehmet/.cargo/registry/src/github.com-1ecc6299db9ec823/rand_core-0.5.1/src/block.rs:343:9
    |
343 |         assert!(index < self.results.as_ref().len());
    |         ^^^^^^

error: cannot find macro `cfg` in this scope
   --> /home/mehmet/.cargo/registry/src/github.com-1ecc6299db9ec823/rand_core-0.5.1/src/block.rs:371:16
    |
371 |             if cfg!(target_endian = "little") {
    |                ^^^
    |
    = note: `cfg` is in scope, but it is an attribute: `#[cfg]`

error: cannot find macro `debug_assert` in this scope
   --> /home/mehmet/.cargo/registry/src/github.com-1ecc6299db9ec823/rand_core-0.5.1/src/impls.rs:61:9
    |
61  |         debug_assert!($N == size_of::<$ty>());
    |         ^^^^^^^^^^^^
...
150 |     impl_uint_from_fill!(rng, u32, 4)
    |     --------------------------------- in this macro invocation
    |
    = note: this error originates in the macro `impl_uint_from_fill` (in Nightly builds, run with -Z macro-backtrace for more info)

error: cannot find macro `debug_assert` in this scope
   --> /home/mehmet/.cargo/registry/src/github.com-1ecc6299db9ec823/rand_core-0.5.1/src/impls.rs:61:9
    |
61  |         debug_assert!($N == size_of::<$ty>());
    |         ^^^^^^^^^^^^
...
155 |     impl_uint_from_fill!(rng, u64, 8)
    |     --------------------------------- in this macro invocation
    |
    = note: this error originates in the macro `impl_uint_from_fill` (in Nightly builds, run with -Z macro-backtrace for more info)

error: cannot find macro `assert_eq` in this scope
  --> /home/mehmet/.cargo/registry/src/github.com-1ecc6299db9ec823/rand_core-0.5.1/src/le.rs:18:9
   |
18 |         assert_eq!($src.len(), $size * $dst.len());
   |         ^^^^^^^^^
...
36 |     read_slice!(src, dst, 4, to_le);
   |     ------------------------------- in this macro invocation
   |
   = note: this error originates in the macro `read_slice` (in Nightly builds, run with -Z macro-backtrace for more info)

error: cannot find macro `assert_eq` in this scope
  --> /home/mehmet/.cargo/registry/src/github.com-1ecc6299db9ec823/rand_core-0.5.1/src/le.rs:18:9
   |
18 |         assert_eq!($src.len(), $size * $dst.len());
   |         ^^^^^^^^^
...
43 |     read_slice!(src, dst, 8, to_le);
   |     ------------------------------- in this macro invocation
   |
   = note: this error originates in the macro `read_slice` (in Nightly builds, run with -Z macro-backtrace for more info)

error: cannot find attribute `test` in this scope
  --> /home/mehmet/.cargo/registry/src/github.com-1ecc6299db9ec823/rand_core-0.5.1/src/le.rs:46:3
   |
46 | #[test]
   |   ^^^^

error: cannot find macro `assert_eq` in this scope
  --> /home/mehmet/.cargo/registry/src/github.com-1ecc6299db9ec823/rand_core-0.5.1/src/le.rs:52:5
   |
52 |     assert_eq!(buf[0], 0x04030201);
   |     ^^^^^^^^^

error: cannot find macro `assert_eq` in this scope
  --> /home/mehmet/.cargo/registry/src/github.com-1ecc6299db9ec823/rand_core-0.5.1/src/le.rs:53:5
   |
53 |     assert_eq!(buf[3], 0x100F0E0D);
   |     ^^^^^^^^^

error: cannot find macro `assert_eq` in this scope
  --> /home/mehmet/.cargo/registry/src/github.com-1ecc6299db9ec823/rand_core-0.5.1/src/le.rs:57:5
   |
57 |     assert_eq!(buf[0], 0x05040302);
   |     ^^^^^^^^^

error: cannot find macro `assert_eq` in this scope
  --> /home/mehmet/.cargo/registry/src/github.com-1ecc6299db9ec823/rand_core-0.5.1/src/le.rs:58:5
   |
58 |     assert_eq!(buf[2], 0x0D0C0B0A);
   |     ^^^^^^^^^

error: cannot find macro `assert_eq` in this scope
  --> /home/mehmet/.cargo/registry/src/github.com-1ecc6299db9ec823/rand_core-0.5.1/src/le.rs:62:5
   |
62 |     assert_eq!(buf[0], 0x0807060504030201);
   |     ^^^^^^^^^

error: cannot find macro `assert_eq` in this scope
  --> /home/mehmet/.cargo/registry/src/github.com-1ecc6299db9ec823/rand_core-0.5.1/src/le.rs:63:5
   |
63 |     assert_eq!(buf[1], 0x100F0E0D0C0B0A09);
   |     ^^^^^^^^^

error: cannot find macro `assert_eq` in this scope
  --> /home/mehmet/.cargo/registry/src/github.com-1ecc6299db9ec823/rand_core-0.5.1/src/le.rs:67:5
   |
67 |     assert_eq!(buf[0], 0x0F0E0D0C0B0A0908);
   |     ^^^^^^^^^

error[E0433]: failed to resolve: use of undeclared crate or module `fmt`
   --> /home/mehmet/.cargo/registry/src/github.com-1ecc6299db9ec823/rand_core-0.5.1/src/error.rs:105:6
    |
105 | impl fmt::Debug for Error {
    |      ^^^ use of undeclared crate or module `fmt`

error[E0433]: failed to resolve: use of undeclared crate or module `fmt`
   --> /home/mehmet/.cargo/registry/src/github.com-1ecc6299db9ec823/rand_core-0.5.1/src/error.rs:106:27
    |
106 |     fn fmt(&self, f: &mut fmt::Formatter) -> fmt::Result {
    |                           ^^^ use of undeclared crate or module `fmt`

error[E0433]: failed to resolve: use of undeclared crate or module `fmt`
   --> /home/mehmet/.cargo/registry/src/github.com-1ecc6299db9ec823/rand_core-0.5.1/src/error.rs:106:46
    |
106 |     fn fmt(&self, f: &mut fmt::Formatter) -> fmt::Result {
    |                                              ^^^ use of undeclared crate or module `fmt`

error[E0433]: failed to resolve: use of undeclared crate or module `fmt`
   --> /home/mehmet/.cargo/registry/src/github.com-1ecc6299db9ec823/rand_core-0.5.1/src/error.rs:119:6
    |
119 | impl fmt::Display for Error {
    |      ^^^ use of undeclared crate or module `fmt`

error[E0433]: failed to resolve: use of undeclared crate or module `fmt`
   --> /home/mehmet/.cargo/registry/src/github.com-1ecc6299db9ec823/rand_core-0.5.1/src/error.rs:120:27
    |
120 |     fn fmt(&self, f: &mut fmt::Formatter) -> fmt::Result {
    |                           ^^^ use of undeclared crate or module `fmt`

error[E0433]: failed to resolve: use of undeclared crate or module `fmt`
   --> /home/mehmet/.cargo/registry/src/github.com-1ecc6299db9ec823/rand_core-0.5.1/src/error.rs:120:46
    |
120 |     fn fmt(&self, f: &mut fmt::Formatter) -> fmt::Result {
    |                                              ^^^ use of undeclared crate or module `fmt`

error[E0433]: failed to resolve: use of undeclared crate or module `fmt`
   --> /home/mehmet/.cargo/registry/src/github.com-1ecc6299db9ec823/rand_core-0.5.1/src/block.rs:122:36
    |
122 | impl<R: BlockRngCore + fmt::Debug> fmt::Debug for BlockRng<R> {
    |                                    ^^^ use of undeclared crate or module `fmt`

error[E0433]: failed to resolve: use of undeclared crate or module `fmt`
   --> /home/mehmet/.cargo/registry/src/github.com-1ecc6299db9ec823/rand_core-0.5.1/src/block.rs:122:24
    |
122 | impl<R: BlockRngCore + fmt::Debug> fmt::Debug for BlockRng<R> {
    |                        ^^^ use of undeclared crate or module `fmt`

error[E0433]: failed to resolve: use of undeclared crate or module `fmt`
   --> /home/mehmet/.cargo/registry/src/github.com-1ecc6299db9ec823/rand_core-0.5.1/src/block.rs:123:29
    |
123 |     fn fmt(&self, fmt: &mut fmt::Formatter) -> fmt::Result {
    |                             ^^^ use of undeclared crate or module `fmt`

error[E0433]: failed to resolve: use of undeclared crate or module `fmt`
   --> /home/mehmet/.cargo/registry/src/github.com-1ecc6299db9ec823/rand_core-0.5.1/src/block.rs:123:48
    |
123 |     fn fmt(&self, fmt: &mut fmt::Formatter) -> fmt::Result {
    |                                                ^^^ use of undeclared crate or module `fmt`

error[E0433]: failed to resolve: use of undeclared crate or module `ptr`
   --> /home/mehmet/.cargo/registry/src/github.com-1ecc6299db9ec823/rand_core-0.5.1/src/block.rs:193:26
    |
193 |                 unsafe { ptr::read_unaligned(ptr) }
    |                          ^^^ use of undeclared crate or module `ptr`

error[E0433]: failed to resolve: use of undeclared crate or module `fmt`
   --> /home/mehmet/.cargo/registry/src/github.com-1ecc6299db9ec823/rand_core-0.5.1/src/block.rs:296:36
    |
296 | impl<R: BlockRngCore + fmt::Debug> fmt::Debug for BlockRng64<R> {
    |                                    ^^^ use of undeclared crate or module `fmt`

error[E0433]: failed to resolve: use of undeclared crate or module `fmt`
   --> /home/mehmet/.cargo/registry/src/github.com-1ecc6299db9ec823/rand_core-0.5.1/src/block.rs:296:24
    |
296 | impl<R: BlockRngCore + fmt::Debug> fmt::Debug for BlockRng64<R> {
    |                        ^^^ use of undeclared crate or module `fmt`

error[E0433]: failed to resolve: use of undeclared crate or module `fmt`
   --> /home/mehmet/.cargo/registry/src/github.com-1ecc6299db9ec823/rand_core-0.5.1/src/block.rs:297:29
    |
297 |     fn fmt(&self, fmt: &mut fmt::Formatter) -> fmt::Result {
    |                             ^^^ use of undeclared crate or module `fmt`

error[E0433]: failed to resolve: use of undeclared crate or module `fmt`
   --> /home/mehmet/.cargo/registry/src/github.com-1ecc6299db9ec823/rand_core-0.5.1/src/block.rs:297:48
    |
297 |     fn fmt(&self, fmt: &mut fmt::Formatter) -> fmt::Result {
    |                                                ^^^ use of undeclared crate or module `fmt`

error[E0433]: failed to resolve: use of undeclared crate or module `slice`
   --> /home/mehmet/.cargo/registry/src/github.com-1ecc6299db9ec823/rand_core-0.5.1/src/impls.rs:66:25
    |
66  |             let slice = slice::from_raw_parts_mut(ptr, $N);
    |                         ^^^^^ use of undeclared crate or module `slice`
...
150 |     impl_uint_from_fill!(rng, u32, 4)
    |     --------------------------------- in this macro invocation
    |
    = note: this error originates in the macro `impl_uint_from_fill` (in Nightly builds, run with -Z macro-backtrace for more info)

error[E0433]: failed to resolve: use of undeclared crate or module `slice`
   --> /home/mehmet/.cargo/registry/src/github.com-1ecc6299db9ec823/rand_core-0.5.1/src/impls.rs:66:25
    |
66  |             let slice = slice::from_raw_parts_mut(ptr, $N);
    |                         ^^^^^ use of undeclared crate or module `slice`
...
155 |     impl_uint_from_fill!(rng, u64, 8)
    |     --------------------------------- in this macro invocation
    |
    = note: this error originates in the macro `impl_uint_from_fill` (in Nightly builds, run with -Z macro-backtrace for more info)

error[E0433]: failed to resolve: use of undeclared crate or module `ptr`
  --> /home/mehmet/.cargo/registry/src/github.com-1ecc6299db9ec823/rand_core-0.5.1/src/le.rs:21:13
   |
21 |             ptr::copy_nonoverlapping(
   |             ^^^ use of undeclared crate or module `ptr`
...
36 |     read_slice!(src, dst, 4, to_le);
   |     ------------------------------- in this macro invocation
   |
   = note: this error originates in the macro `read_slice` (in Nightly builds, run with -Z macro-backtrace for more info)

error[E0433]: failed to resolve: use of undeclared crate or module `ptr`
  --> /home/mehmet/.cargo/registry/src/github.com-1ecc6299db9ec823/rand_core-0.5.1/src/le.rs:21:13
   |
21 |             ptr::copy_nonoverlapping(
   |             ^^^ use of undeclared crate or module `ptr`
...
43 |     read_slice!(src, dst, 8, to_le);
   |     ------------------------------- in this macro invocation
   |
   = note: this error originates in the macro `read_slice` (in Nightly builds, run with -Z macro-backtrace for more info)

error[E0412]: cannot find type `NonZeroU32` in this scope
  --> /home/mehmet/.cargo/registry/src/github.com-1ecc6299db9ec823/rand_core-0.5.1/src/error.rs:24:11
   |
24 |     code: NonZeroU32,
   |           ^^^^^^^^^^ not found in this scope

error[E0412]: cannot find type `Option` in this scope
  --> /home/mehmet/.cargo/registry/src/github.com-1ecc6299db9ec823/rand_core-0.5.1/src/error.rs:76:35
   |
76 |     pub fn raw_os_error(&self) -> Option<i32> {
   |                                   ^^^^^^ not found in this scope

error[E0531]: cannot find tuple struct or tuple variant `Some` in this scope
  --> /home/mehmet/.cargo/registry/src/github.com-1ecc6299db9ec823/rand_core-0.5.1/src/error.rs:83:13
   |
83 |             Some(code) if u32::from(code) < Self::INTERNAL_START =>
   |             ^^^^ not found in this scope

error[E0425]: cannot find function, tuple struct or tuple variant `Some` in this scope
  --> /home/mehmet/.cargo/registry/src/github.com-1ecc6299db9ec823/rand_core-0.5.1/src/error.rs:84:17
   |
84 |                 Some(u32::from(code) as i32),
   |                 ^^^^ not found in this scope

error[E0425]: cannot find value `None` in this scope
  --> /home/mehmet/.cargo/registry/src/github.com-1ecc6299db9ec823/rand_core-0.5.1/src/error.rs:85:18
   |
85 |             _ => None,
   |                  ^^^^ not found in this scope

error[E0412]: cannot find type `Option` in this scope
  --> /home/mehmet/.cargo/registry/src/github.com-1ecc6299db9ec823/rand_core-0.5.1/src/error.rs:95:27
   |
95 |     pub fn code(&self) -> Option<NonZeroU32> {
   |                           ^^^^^^ not found in this scope

error[E0412]: cannot find type `NonZeroU32` in this scope
  --> /home/mehmet/.cargo/registry/src/github.com-1ecc6299db9ec823/rand_core-0.5.1/src/error.rs:95:34
   |
27 | impl Error {
   |     - help: you might be missing a type parameter: `<NonZeroU32>`
...
95 |     pub fn code(&self) -> Option<NonZeroU32> {
   |                                  ^^^^^^^^^^ not found in this scope

error[E0425]: cannot find function, tuple struct or tuple variant `Some` in this scope
   --> /home/mehmet/.cargo/registry/src/github.com-1ecc6299db9ec823/rand_core-0.5.1/src/error.rs:100:13
    |
100 |             Some(self.code)
    |             ^^^^ not found in this scope

error[E0405]: cannot find trait `From` in this scope
   --> /home/mehmet/.cargo/registry/src/github.com-1ecc6299db9ec823/rand_core-0.5.1/src/error.rs:133:6
    |
133 | impl From<NonZeroU32> for Error {
    |      ^^^^ not found in this scope

error[E0412]: cannot find type `NonZeroU32` in this scope
   --> /home/mehmet/.cargo/registry/src/github.com-1ecc6299db9ec823/rand_core-0.5.1/src/error.rs:133:11
    |
133 | impl From<NonZeroU32> for Error {
    |     -     ^^^^^^^^^^ not found in this scope
    |     |
    |     help: you might be missing a type parameter: `<NonZeroU32>`

error[E0412]: cannot find type `NonZeroU32` in this scope
   --> /home/mehmet/.cargo/registry/src/github.com-1ecc6299db9ec823/rand_core-0.5.1/src/error.rs:135:19
    |
135 |     fn from(code: NonZeroU32) -> Self {
    |                   ^^^^^^^^^^ not found in this scope

error[E0405]: cannot find trait `AsRef` in this scope
  --> /home/mehmet/.cargo/registry/src/github.com-1ecc6299db9ec823/rand_core-0.5.1/src/block.rs:70:19
   |
70 |     type Results: AsRef<[Self::Item]> + AsMut<[Self::Item]> + Default;
   |                   ^^^^^ not found in this scope

error[E0405]: cannot find trait `AsMut` in this scope
  --> /home/mehmet/.cargo/registry/src/github.com-1ecc6299db9ec823/rand_core-0.5.1/src/block.rs:70:41
   |
70 |     type Results: AsRef<[Self::Item]> + AsMut<[Self::Item]> + Default;
   |                                         ^^^^^ not found in this scope

error[E0405]: cannot find trait `Default` in this scope
  --> /home/mehmet/.cargo/registry/src/github.com-1ecc6299db9ec823/rand_core-0.5.1/src/block.rs:70:63
   |
70 |     type Results: AsRef<[Self::Item]> + AsMut<[Self::Item]> + Default;
   |                                                               ^^^^^^^ not found in this scope

error[E0405]: cannot find trait `Sized` in this scope
   --> /home/mehmet/.cargo/registry/src/github.com-1ecc6299db9ec823/rand_core-0.5.1/src/block.rs:114:40
    |
114 | pub struct BlockRng<R: BlockRngCore + ?Sized> {
    |                                        ^^^^^ not found in this scope

error[E0405]: cannot find trait `AsRef` in this scope
   --> /home/mehmet/.cargo/registry/src/github.com-1ecc6299db9ec823/rand_core-0.5.1/src/block.rs:173:37
    |
173 | where <R as BlockRngCore>::Results: AsRef<[u32]> + AsMut<[u32]>
    |                                     ^^^^^ not found in this scope

error[E0405]: cannot find trait `AsMut` in this scope
   --> /home/mehmet/.cargo/registry/src/github.com-1ecc6299db9ec823/rand_core-0.5.1/src/block.rs:173:52
    |
173 | where <R as BlockRngCore>::Results: AsRef<[u32]> + AsMut<[u32]>
    |                                                    ^^^^^ not found in this scope

error[E0412]: cannot find type `Result` in this scope
   --> /home/mehmet/.cargo/registry/src/github.com-1ecc6299db9ec823/rand_core-0.5.1/src/block.rs:236:54
    |
236 |     fn try_fill_bytes(&mut self, dest: &mut [u8]) -> Result<(), Error> {
    |                                                      ^^^^^^ not found in this scope

error[E0425]: cannot find function, tuple struct or tuple variant `Ok` in this scope
   --> /home/mehmet/.cargo/registry/src/github.com-1ecc6299db9ec823/rand_core-0.5.1/src/block.rs:238:9
    |
238 |         Ok(())
    |         ^^ not found in this scope

error[E0412]: cannot find type `Result` in this scope
   --> /home/mehmet/.cargo/registry/src/github.com-1ecc6299db9ec823/rand_core-0.5.1/src/block.rs:256:40
    |
256 |     fn from_rng<S: RngCore>(rng: S) -> Result<Self, Error> {
    |                                        ^^^^^^ not found in this scope

error[E0425]: cannot find function, tuple struct or tuple variant `Ok` in this scope
   --> /home/mehmet/.cargo/registry/src/github.com-1ecc6299db9ec823/rand_core-0.5.1/src/block.rs:257:9
    |
257 |         Ok(Self::new(R::from_rng(rng)?))
    |         ^^ not found in this scope

error[E0405]: cannot find trait `Sized` in this scope
   --> /home/mehmet/.cargo/registry/src/github.com-1ecc6299db9ec823/rand_core-0.5.1/src/block.rs:287:42
    |
287 | pub struct BlockRng64<R: BlockRngCore + ?Sized> {
    |                                          ^^^^^ not found in this scope

error[E0405]: cannot find trait `AsRef` in this scope
   --> /home/mehmet/.cargo/registry/src/github.com-1ecc6299db9ec823/rand_core-0.5.1/src/block.rs:351:37
    |
351 | where <R as BlockRngCore>::Results: AsRef<[u64]> + AsMut<[u64]>
    |                                     ^^^^^ not found in this scope

error[E0405]: cannot find trait `AsMut` in this scope
   --> /home/mehmet/.cargo/registry/src/github.com-1ecc6299db9ec823/rand_core-0.5.1/src/block.rs:351:52
    |
351 | where <R as BlockRngCore>::Results: AsRef<[u64]> + AsMut<[u64]>
    |                                                    ^^^^^ not found in this scope

error[E0412]: cannot find type `Result` in this scope
   --> /home/mehmet/.cargo/registry/src/github.com-1ecc6299db9ec823/rand_core-0.5.1/src/block.rs:412:54
    |
412 |     fn try_fill_bytes(&mut self, dest: &mut [u8]) -> Result<(), Error> {
    |                                                      ^^^^^^ not found in this scope

error[E0425]: cannot find function, tuple struct or tuple variant `Ok` in this scope
   --> /home/mehmet/.cargo/registry/src/github.com-1ecc6299db9ec823/rand_core-0.5.1/src/block.rs:414:9
    |
414 |         Ok(())
    |         ^^ not found in this scope

error[E0412]: cannot find type `Result` in this scope
   --> /home/mehmet/.cargo/registry/src/github.com-1ecc6299db9ec823/rand_core-0.5.1/src/block.rs:432:40
    |
432 |     fn from_rng<S: RngCore>(rng: S) -> Result<Self, Error> {
    |                                        ^^^^^^ not found in this scope

error[E0425]: cannot find function, tuple struct or tuple variant `Ok` in this scope
   --> /home/mehmet/.cargo/registry/src/github.com-1ecc6299db9ec823/rand_core-0.5.1/src/block.rs:433:9
    |
433 |         Ok(Self::new(R::from_rng(rng)?))
    |         ^^ not found in this scope

error[E0405]: cannot find trait `Sized` in this scope
  --> /home/mehmet/.cargo/registry/src/github.com-1ecc6299db9ec823/rand_core-0.5.1/src/impls.rs:28:39
   |
28 | pub fn next_u64_via_u32<R: RngCore + ?Sized>(rng: &mut R) -> u64 {
   |                                       ^^^^^ not found in this scope

error[E0405]: cannot find trait `Sized` in this scope
  --> /home/mehmet/.cargo/registry/src/github.com-1ecc6299db9ec823/rand_core-0.5.1/src/impls.rs:41:42
   |
41 | pub fn fill_bytes_via_next<R: RngCore + ?Sized>(rng: &mut R, dest: &mut [u8]) {
   |                                          ^^^^^ not found in this scope

error[E0425]: cannot find function `min` in this scope
   --> /home/mehmet/.cargo/registry/src/github.com-1ecc6299db9ec823/rand_core-0.5.1/src/impls.rs:75:29
    |
75  |         let chunk_size_u8 = min($src.len() * $size, $dst.len());
    |                             ^^^ not found in this scope
...
131 |     fill_via_chunks!(src, dest, u32, 4)
    |     ----------------------------------- in this macro invocation
    |
    = note: this error originates in the macro `fill_via_chunks` (in Nightly builds, run with -Z macro-backtrace for more info)

error[E0425]: cannot find function `copy_nonoverlapping` in this scope
   --> /home/mehmet/.cargo/registry/src/github.com-1ecc6299db9ec823/rand_core-0.5.1/src/impls.rs:79:17
    |
79  |                 copy_nonoverlapping(
    |                 ^^^^^^^^^^^^^^^^^^^ not found in this scope
...
131 |     fill_via_chunks!(src, dest, u32, 4)
    |     ----------------------------------- in this macro invocation
    |
    = note: this error originates in the macro `fill_via_chunks` (in Nightly builds, run with -Z macro-backtrace for more info)

error[E0425]: cannot find function `copy_nonoverlapping` in this scope
   --> /home/mehmet/.cargo/registry/src/github.com-1ecc6299db9ec823/rand_core-0.5.1/src/impls.rs:89:21
    |
89  |                     copy_nonoverlapping(src_ptr,
    |                     ^^^^^^^^^^^^^^^^^^^ not found in this scope
...
131 |     fill_via_chunks!(src, dest, u32, 4)
    |     ----------------------------------- in this macro invocation
    |
    = note: this error originates in the macro `fill_via_chunks` (in Nightly builds, run with -Z macro-backtrace for more info)

error[E0425]: cannot find function `min` in this scope
   --> /home/mehmet/.cargo/registry/src/github.com-1ecc6299db9ec823/rand_core-0.5.1/src/impls.rs:75:29
    |
75  |         let chunk_size_u8 = min($src.len() * $size, $dst.len());
    |                             ^^^ not found in this scope
...
145 |     fill_via_chunks!(src, dest, u64, 8)
    |     ----------------------------------- in this macro invocation
    |
    = note: this error originates in the macro `fill_via_chunks` (in Nightly builds, run with -Z macro-backtrace for more info)

error[E0425]: cannot find function `copy_nonoverlapping` in this scope
   --> /home/mehmet/.cargo/registry/src/github.com-1ecc6299db9ec823/rand_core-0.5.1/src/impls.rs:79:17
    |
79  |                 copy_nonoverlapping(
    |                 ^^^^^^^^^^^^^^^^^^^ not found in this scope
...
145 |     fill_via_chunks!(src, dest, u64, 8)
    |     ----------------------------------- in this macro invocation
    |
    = note: this error originates in the macro `fill_via_chunks` (in Nightly builds, run with -Z macro-backtrace for more info)

error[E0425]: cannot find function `copy_nonoverlapping` in this scope
   --> /home/mehmet/.cargo/registry/src/github.com-1ecc6299db9ec823/rand_core-0.5.1/src/impls.rs:89:21
    |
89  |                     copy_nonoverlapping(src_ptr,
    |                     ^^^^^^^^^^^^^^^^^^^ not found in this scope
...
145 |     fill_via_chunks!(src, dest, u64, 8)
    |     ----------------------------------- in this macro invocation
    |
    = note: this error originates in the macro `fill_via_chunks` (in Nightly builds, run with -Z macro-backtrace for more info)

error[E0405]: cannot find trait `Sized` in this scope
   --> /home/mehmet/.cargo/registry/src/github.com-1ecc6299db9ec823/rand_core-0.5.1/src/impls.rs:149:40
    |
149 | pub fn next_u32_via_fill<R: RngCore + ?Sized>(rng: &mut R) -> u32 {
    |                                        ^^^^^ not found in this scope

error[E0405]: cannot find trait `Sized` in this scope
   --> /home/mehmet/.cargo/registry/src/github.com-1ecc6299db9ec823/rand_core-0.5.1/src/impls.rs:154:40
    |
154 | pub fn next_u64_via_fill<R: RngCore + ?Sized>(rng: &mut R) -> u64 {
    |                                        ^^^^^ not found in this scope

error[E0412]: cannot find type `Result` in this scope
   --> /home/mehmet/.cargo/registry/src/github.com-1ecc6299db9ec823/rand_core-0.5.1/src/lib.rs:183:54
    |
183 |     fn try_fill_bytes(&mut self, dest: &mut [u8]) -> Result<(), Error>;
    |                                                      ^^^^^^ not found in this scope

error[E0405]: cannot find trait `Sized` in this scope
   --> /home/mehmet/.cargo/registry/src/github.com-1ecc6299db9ec823/rand_core-0.5.1/src/lib.rs:216:24
    |
216 | pub trait SeedableRng: Sized {
    |                        ^^^^^ not found in this scope

error[E0405]: cannot find trait `Sized` in this scope
   --> /home/mehmet/.cargo/registry/src/github.com-1ecc6299db9ec823/rand_core-0.5.1/src/lib.rs:262:16
    |
262 |     type Seed: Sized + Default + AsMut<[u8]>;
    |                ^^^^^ not found in this scope

error[E0405]: cannot find trait `Default` in this scope
   --> /home/mehmet/.cargo/registry/src/github.com-1ecc6299db9ec823/rand_core-0.5.1/src/lib.rs:262:24
    |
262 |     type Seed: Sized + Default + AsMut<[u8]>;
    |                        ^^^^^^^ not found in this scope

error[E0405]: cannot find trait `AsMut` in this scope
   --> /home/mehmet/.cargo/registry/src/github.com-1ecc6299db9ec823/rand_core-0.5.1/src/lib.rs:262:34
    |
262 |     type Seed: Sized + Default + AsMut<[u8]>;
    |                                  ^^^^^ not found in this scope

error[E0425]: cannot find function `copy_nonoverlapping` in this scope
   --> /home/mehmet/.cargo/registry/src/github.com-1ecc6299db9ec823/rand_core-0.5.1/src/lib.rs:323:17
    |
323 |                 copy_nonoverlapping(p, chunk.as_mut_ptr(), chunk.len());
    |                 ^^^^^^^^^^^^^^^^^^^ not found in this scope

error[E0412]: cannot find type `Result` in this scope
   --> /home/mehmet/.cargo/registry/src/github.com-1ecc6299db9ec823/rand_core-0.5.1/src/lib.rs:355:44
    |
355 |     fn from_rng<R: RngCore>(mut rng: R) -> Result<Self, Error> {
    |                                            ^^^^^^ not found in this scope

error[E0425]: cannot find function, tuple struct or tuple variant `Ok` in this scope
   --> /home/mehmet/.cargo/registry/src/github.com-1ecc6299db9ec823/rand_core-0.5.1/src/lib.rs:358:9
    |
358 |         Ok(Self::from_seed(seed))
    |         ^^ not found in this scope

error[E0405]: cannot find trait `Sized` in this scope
   --> /home/mehmet/.cargo/registry/src/github.com-1ecc6299db9ec823/rand_core-0.5.1/src/lib.rs:388:24
    |
388 | impl<'a, R: RngCore + ?Sized> RngCore for &'a mut R {
    |                        ^^^^^ not found in this scope

error[E0412]: cannot find type `Result` in this scope
   --> /home/mehmet/.cargo/registry/src/github.com-1ecc6299db9ec823/rand_core-0.5.1/src/lib.rs:405:54
    |
405 |     fn try_fill_bytes(&mut self, dest: &mut [u8]) -> Result<(), Error> {
    |                                                      ^^^^^^ not found in this scope

error[E0405]: cannot find trait `Sized` in this scope
   --> /home/mehmet/.cargo/registry/src/github.com-1ecc6299db9ec823/rand_core-0.5.1/src/lib.rs:445:26
    |
445 | impl<'a, R: CryptoRng + ?Sized> CryptoRng for &'a mut R {}
    |                          ^^^^^ not found in this scope

Some errors have detailed explanations: E0405, E0412, E0425, E0433, E0463, E0531.
For more information about an error, try `rustc --explain E0405`.
error: could not compile `rand_core` due to 104 previous errors
warning: build failed, waiting for other jobs to finish...
error: build failed
make: *** [Makefile:5: build-contract] Error 101
