# rust-sveltekit

Example project embedding Sveltekit application into Rust binary at compile time

## Description

This repo is meant to show how to embed a Sveltekit application within a Rust binary using the [Rust Embed crate](https://crates.io/crates/rust-embed)

## Install

```bash
# Build UI (from project root)
cd ui
npm i
npm run build

# Build binary (from project root)
cargo run

```

## Notes

- The Sveltekit application uses the `static-adapter` and places its build artifacts in `ui/build`
- This repo uses `axum` as the web application framework
  - The code for the `main.rs` is taken from [the `axum` example from the Rust Embed repo](https://github.com/pyrossh/rust-embed/blob/master/examples/axum-spa/main.rs)
