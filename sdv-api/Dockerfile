FROM rust:1.82.0 AS builder

WORKDIR /usr/src/sdv-api
COPY . .

RUN cargo build --release


FROM debian:12.7-slim AS prod

COPY --from=builder /usr/src/sdv-api/target/release/sdv-api /usr/local/bin/sdv-api

CMD ["sdv-api"]
