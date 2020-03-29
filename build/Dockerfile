FROM rust:buster as builder
WORKDIR /app
RUN git clone https://github.com/paritytech/substrate-telemetry.git
RUN cd substrate-telemetry && git checkout 85b78095333cc9b767e4618e4f3457abe46e4a5e
RUN cp -rf substrate-telemetry/backend/* .
RUN cargo build --release

FROM rust:slim-buster
WORKDIR /app

COPY --from=builder /app/target/release/telemetry /usr/local/bin/

EXPOSE 8000

ENTRYPOINT [ "telemetry" ]

