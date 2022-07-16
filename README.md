# KyattsuChain
Blockchain Infrastructure for Kyattsu Network

Built On Parity [Substrate](https://github.com/paritytech/substrate)

## Build

```bash
sudo apt install build-essential

sudo apt install --assume-yes git clang curl libssl-dev llvm libudev-dev make protobuf-compiler

curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh

source $HOME/.cargo/env

rustup default stable
rustup update

rustup update nightly
rustup target add wasm32-unknown-unknown --toolchain nightly

git clone --recursive https://github.com/KyattsuNetwork/KyattsuChain

cd KyattsuChain

cargo build --release
```

## Run

```
./kyattsu-chain-node
```