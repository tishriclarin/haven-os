# Code and documentation style
Rust-first for original security services. Favor small modules, typed errors, explicit ownership, bounded input and narrow privileges. Avoid unsafe code unless justified by an ADR and focused review.

When Rust code exists, use cargo fmt, cargo clippy and cargo test. Test trust boundaries and adversarial behavior rather than implementation trivia. Audit dependencies and lock release dependencies. These checks are planned; no Rust code exists yet.

Documentation distinguishes proposed, prototyped, verified and released behavior. Use concrete limits; never claim perfect isolation or guaranteed revocation.
