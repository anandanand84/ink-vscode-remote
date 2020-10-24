FROM rustlang/rust:nightly
RUN rustup component add rust-src --toolchain nightly
RUN rustup target add wasm32-unknown-unknown --toolchain stable
RUN rustup install nightly-2020-10-06
RUN rustup target add wasm32-unknown-unknown --toolchain nightly-2020-10-06
RUN cargo +nightly-2020-10-06 install canvas-node --git https://github.com/paritytech/canvas-node.git --tag v0.1.0 --force
RUN cargo install cargo-contract --vers 0.7.0 --force
