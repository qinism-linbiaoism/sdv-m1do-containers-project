FROM rust:1.82.0

WORKDIR /usr/src/sdv-api
COPY . .

RUN cargo build --release

EXPOSE 8000

CMD ["./target/release/sdv-api"]
