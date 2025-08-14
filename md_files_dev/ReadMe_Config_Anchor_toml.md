ReadMe_Anchor_toml.md


Yes, that would be smart to align everything properly. Here’s the recommended pairing for **Rust 1.79.0** (a stable choice for Anchor right now):

✅ **Rust:** `1.79.0` (stable, avoids edition2024 problems)
✅ **Anchor CLI:** `0.31.1` (current stable release)
✅ **Solana CLI:** `1.18.x` (e.g., `1.18.10`)

These versions work well together because:

* **Anchor 0.31.x** officially supports Solana 1.18.x.
* Rust 1.79.0 is stable and compatible with all Anchor/Solana crates without pulling in `edition2024`.

---

If your Solana CLI is newer than `1.18.x` (like `2.x.x`), you **must downgrade** to `1.18.x` for Anchor 0.31.x, or upgrade Anchor to an unreleased dev branch (not recommended for production).

Want me to give you **the exact commands to:**

* Remove nightly override
* Set Rust to 1.79.0
* Install the matching Solana & Anchor versions
* Verify everything is synced?


