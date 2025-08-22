ReadMe_Config_Rust-Toolchain_toml.md

# this file is to manage rust based package and tool chain
# refer anchor.toml to configure any version mismatch between anchor/solana/rust

[toolchain]
channel = "1.79.0"
#"nightly"
#"1.79.0"
components = ["rust-src", "llvm-tools-preview"]
targets = ["bpfel-unknown-unknown"]
profile = "minimal"

Installed Versions:
Rust: rustc 1.86.0 (05f9846f8 2025-03-31)
Solana CLI: solana-cli 2.2.12 (src:0315eb6a; feat:1522022101, client:Agave)
Anchor CLI: anchor-cli 0.31.1
Node.js: v23.11.0
Yarn: 1.22.1

