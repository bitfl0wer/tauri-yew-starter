## Setting up a dev environment

Add wasm as a compilation target

```
rustup target add wasm32-unknown-unknown
```

Install `tauri-cli` and `trunk`
```sh
cargo install tauri-cli trunk --locked
```

To start the web-based application, change into the `crates/polyphony-wasm` directory and run `trunk serve`.

To start the Tauri powered Desktop-App instead, change into the `crates/polyphony-tauri` directory and run `cargo tauri dev`. 

> Note that the Tauri Dev Server will try to run and listen for the `trunk serve` Dev server. If it fails to do so (perhaps because Port `8080` is already occupied), it will not be able to start the Tauri App.

