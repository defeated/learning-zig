# syntax=docker/dockerfile:1
# use base devcontainer image on alpine
ARG ALPINE_VERSION=3.20
FROM mcr.microsoft.com/vscode/devcontainers/base:alpine-${ALPINE_VERSION}

# upgrade to edge branch
ARG ALPINE_VERSION
RUN sed -ie s/v${ALPINE_VERSION}/edge/ /etc/apk/repositories

# install zig & zig language server
ARG ZIG_VERSION=0.13.0
RUN apk add --update-cache zig=~${ZIG_VERSION} zls=~${ZIG_VERSION}

CMD ["zig", "version"]
