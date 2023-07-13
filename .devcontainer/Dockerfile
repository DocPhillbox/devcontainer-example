ARG VARIANT="jammy"
FROM mcr.microsoft.com/vscode/devcontainers/base:0-${VARIANT}

RUN apt update && export DEBIAN_FRONTEND=noninteractive && yes | unminimize && \
    apt --only-upgrade install apt libapt-pkg6.0  libgnutls30 && \
    apt install -y gdb