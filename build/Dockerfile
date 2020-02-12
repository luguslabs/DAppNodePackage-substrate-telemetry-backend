FROM rust:buster as builder
WORKDIR /app
RUN git clone https://github.com/paritytech/substrate-telemetry.git
RUN cd substrate-telemetry && git checkout b665555de6cdfd5a1908ded62ef0b3fca7ab1430
RUN cp -rf substrate-telemetry/backend/* .
RUN cargo build --release

FROM rust:slim-buster
WORKDIR /app

COPY --from=builder /app/target/release/telemetry /usr/local/bin/

EXPOSE 8000

ENTRYPOINT [ "telemetry" ]

