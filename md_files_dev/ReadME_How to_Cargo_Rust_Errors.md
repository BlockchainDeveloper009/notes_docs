ReadME_How to_Cargo_Errors.md

arishgk@harishgk-HP-EliteBook-840-G3:~/source/repos/defi_lending_protocol_sol/lending_backend_solana$ cargo tree | grep base64ct
harishgk@harishgk-HP-EliteBook-840-G3:~/source/repos/defi_lending_protocol_sol/lending_backend_solana$ cargo update -p base64ct@1.8.0 --precise 1.7.3
    Updating crates.io index
 Downgrading base64ct v1.8.0 -> v1.7.3
note: pass `--verbose` to see 2 unchanged dependencies behind latest
harishgk@harishgk-HP-EliteBook-840-G3:~/source/repos/defi_lending_protocol_sol/lending_```
backend_solana$ cargo tree | grep base64ct
  Downloaded base64ct v1.7.3
  Downloaded 1 crate (30.4KiB) in 0.52s
harishgk@harishgk-HP-EliteBook-840-G3:~/source/repos/defi_lending_protocol_sol/lending_backend_solana$ anchor build
  Downloaded base16ct v0.2.0
  Downloaded base64ct v1.7.3
  ```

rustup show
rustc --version

rustup target list --installed

rustup install stable
rustup default stable
rustup update

rustup component add rust-std --toolchain nightly --target x86_64-unknown-linux-gnu

rustup component add rust-std --toolchain stable --target x86_64-unknown-linux-gnu



anchor.toml
cargo.toml (workspace level)
[patch.crates-io]
base64ct = "=1.7.3"



cargo.toml (smart contract folder level)

[dependencies]
base64ct = "=1.7.3"


#### Cargo level:

cargo update -p base64ct@1.8.0 --precise 1.7.3
cargo tree | grep base64ct

cargo tree | grep pyth


## RUST LEVL ERRORS:

export RUSTC_BOOTSTRAP=1

TO SETUP NIGHTLY RUN

```
rustup install nightly
rustup override set nightly

rustup install 1.79.0 --force
rustup default 1.79.0
rustup component add rust-src
rustup component add rust-std
rustup component add rust-std
rustup component add rustc-dev
rustup component add llvm-tools-preview

rustup install nightly
rustup override set nightly
rustc --version  # should show nightly
anchor build

```


### Cargo cleanup:
cargo clean

cargo clean
cargo update
anchor build


### Cache clearing

anchor clean cache
cargo clean cache

rustup target add bpfel-unknown-unknown
rustup target add x86_64-unknown-linux-gnu


$ rustup show
 	```
 	Default host: x86_64-unknown-linux-gnu
rustup home:  /home/harishgk/.rustup

installed toolchains
--------------------
stable-x86_64-unknown-linux-gnu (default)
nightly-x86_64-unknown-linux-gnu (active)
solana

active toolchain
----------------
name: nightly-x86_64-unknown-linux-gnu
active because: directory override for '/home/harishgk/source/repos/defi_lending_protocol_sol/lending_backend_solana'
installed targets:
  x86_64-unknown-linux-gnu
harishgk@harishgk-HP-EliteBook-8
 	```


$ rustup target list --installed
x86_64-unknown-linux-gnu

$ rustc  --version
rustc 1.91.0-nightly (3672a55b7 2025-08-13)


### Rust_Error:
------------
```

rustup component add rust-std rustfmt clippy

```


to setup rust version
---------------------
$ rustup override set 1.79.0 
-----------------------------
```
info: syncing channel updates for '1.79.0-x86_64-unknown-linux-gnu'
info: latest update on 2024-06-13, rust version 1.79.0 (129f3b996 2024-06-10)

  1.79.0-x86_64-unknown-linux-gnu installed - rustc 1.79.0 (129f3b996 2024-06-10)

info: override toolchain for '/home/harishgk/source/repos/defi_lending_protocol_sol/lending_backend_solana' set to '1.79.0-x86_64-unknown-linux-gnu'
harishgk@harishgk-HP-EliteBook-840-G3:~/source/repos/defi_lending_protocol_sol/lending_backend_solana$ rustup show
Default host: x86_64-unknown-linux-gnu
rustup home:  /home/harishgk/.rustup

```
installed toolchains
--------------------
stable-x86_64-unknown-linux-gnu (default)
nightly-x86_64-unknown-linux-gnu
1.79.0-x86_64-unknown-linux-gnu (active)
solana

active toolchain
----------------
name: 1.79.0-x86_64-unknown-linux-gnu
active because: directory override for '/home/harishgk/source/repos/defi_lending_protocol_sol/lending_backend_solana'
installed targets:
  x86_64-unknown-linux-gnu
harishgk@harishgk-HP-EliteBook-840-G3:~/source/repos/defi_lending_protocol_sol/lending_backend_solana$ 




anchor build_Error1: error[E0463]: can't find crate for `core`
-------

```
_solana$ anchor build
   Compiling proc-macro2 v1.0.97
   Compiling unicode-ident v1.0.18
   Compiling serde v1.0.219
   Compiling hashbrown v0.15.5
error[E0463]: can't find crate for `core`
  |
  = note: the `x86_64-unknown-linux-gnu` target may not be installed
  = help: consider adding the standard library to the sysroot with `x build library --target x86_64-unknown-linux-gnu`
  = help: consider building the standard library from source with `cargo build -Zbuild-std`

For more information about this error, try `rustc --explain E0463`.
error: could not compile `unicode-ident` (lib) due to 1 previous error
warning: build failed, waiting for other jobs to finish...
error[E0463]: can't find crate for `std`
  |
  = note: the `x86_64-unknown-linux-gnu` target may not be installed
  = help: consider adding the standard library to the sysroot with `x build library --target x86_64-unknown-linux-gnu`
  = help: consider building the standard library from source with `cargo build -Zbuild-std`

error: could not compile `proc-macro2` (build script) due to 1 previous error
error: could not compile `serde` (build script) due to 1 previous error
error: could not compile `hashbrown` (lib) due to 1 previous error
harishgk@harishgk-HP-EliteBook-840-G3:~/source/repos/defi_lending_protocol_sol/lending_backend_solana$ 

```

anchor build_Error1:Solution
---------------------------- 
``` 

```




anchor2
-------