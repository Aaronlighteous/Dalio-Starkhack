## Getting Started

Follow the steps below to get started with Madara :hammer_and_wrench:

### Madara Setup

Madara can be a bit tricky by requiring rustup installer for a nightly build.
Took my time to run wihtout errors.

Install rustc 1.69.0-nightly

```bash
curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh
```

```bash
rustup toolchain install nightly
```

Install nvm latest

```bash
curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.39.3/install.sh | bash
```

Install Cairo 1.0

```bash
curl -L https://github.com/franalgaba/cairo-installer/raw/main/bin/cairo-installer | bash
```

protobuf for buildtime (If you don't have it you will HAVE errors)

```bash
brew install protobuf
```

For madara if our repo doesn't work you can just build on the root folder, but our repo should work

```bash
cd ~
git clone https://github.com/keep-starknet-strange/madara.git
```

Then build (this may get around 3-15 minutes)

```bash
cd madara
cargo build --release
```

Run madara with our config

```bash
./target/release/madara setup --chain dev --from-local ./configs
```

### Contracts

We have another contracts folder to easily see what contributions we have made or in case of not being able to run Madara from our repo, you can add these contracts to Madara with our configuration to have our project locally.

## Demo

TBA
