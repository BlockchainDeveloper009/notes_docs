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

```


### Cargo cleanup:
cargo clean

rustup install 1.79.0 --force
rustup default 1.79.0
rustup component add rust-src
rustup component add rust-std

### Cache clearing

anchor clean cache
cargo clean cache