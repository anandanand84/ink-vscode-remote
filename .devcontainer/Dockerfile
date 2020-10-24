FROM rustlang/rust:nightly
RUN rustup component add rust-src --toolchain nightly
RUN rustup install nightly-2020-10-06
RUN rustup target add wasm32-unknown-unknown --toolchain nightly-2020-10-06
RUN apt-get update -y && apt-get install -y libclang-dev clang
RUN cargo +nightly-2020-10-06 install canvas-node --git https://github.com/paritytech/canvas-node.git --tag v0.1.0 --force
RUN cargo +nightly-2020-10-06 install cargo-contract --vers 0.7.0 --force
RUN rustup default nightly
EXPOSE 9944
EXPOSE 9615
