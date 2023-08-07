# syntax=docker/dockerfile:1.4


# Base Image
# =============================================================================
# Start from a Rust base image
FROM rust:latest

# Install dependencies for Substrate
RUN apt-get update && \
    apt-get upgrade -y && \
    apt-get install -y cmake pkg-config libssl-dev git clang curl

# Install wasm toolchain
RUN curl https://getsubstrate.io -sSf | bash -s -- --fast

# Add source files to container (optional)
# ADD . /your-app

# Set the workdir (optional)
# WORKDIR /your-app

# Build your app (optional)
# RUN cargo build --release
