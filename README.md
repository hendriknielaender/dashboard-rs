# dashboard-rs
leptos + tailwind

Install Tailwind and build the CSS:

`npx tailwindcss -i ./input.css -o ./style/output.css --watch`

Install trunk to client side render this bundle.

`cargo install trunk`
Then the site can be served with `trunk serve --open`

The browser will automatically open [http://127.0.0.1:8080//](http://127.0.0.1:8080//)

You can begin editing your app at `src/app.rs`.

## Installing Tailwind

You can install Tailwind using `npm`:

```bash
npm install -D tailwindcss
```

If you'd rather not use `npm`, you can install the Tailwind binary [here](https://github.com/tailwindlabs/tailwindcss/releases).

## Notes about Tooling

By default, `cargo-leptos` uses `nightly` Rust, `cargo-generate`, and `sass`. If you run into any trouble, you may need to install one or more of these tools.

1. `rustup toolchain install nightly --allow-downgrade` - make sure you have Rust nightly
2. `rustup default nightly` - setup nightly as default, or you can use rust-toolchain file later on
3. `rustup target add wasm32-unknown-unknown` - add the ability to compile Rust to WebAssembly
4. `cargo install cargo-generate` - install `cargo-generate` binary (should be installed automatically in future)
5. `npm install -g sass` - install `dart-sass` (should be optional in future

