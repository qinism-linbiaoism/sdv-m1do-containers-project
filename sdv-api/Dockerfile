FROM rust:1.82.0

WORKDIR /usr/src/sdv-api
COPY . .

RUN cargo build --release

CMD ["./target/release/sdv-api"]
