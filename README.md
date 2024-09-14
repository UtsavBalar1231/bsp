# bsp - Radxa BSP Build Tool

[![Build](https://github.com/radxa-repo/bsp/actions/workflows/build.yml/badge.svg)](https://github.com/radxa-repo/bsp/actions/workflows/build.yml)

`bsp` aims to provide a standardized way to build Linux kernel and U-Boot for Radxa boards, so the build output can be easliy included in our image generation pipeline.

## Dependencies

> Ubuntu 22.04 / Debian 12

```
sudo apt update
sudo apt install -y git qemu-user-static binfmt-support

# Podman (recommended)
sudo apt install -y podman podman-docker
sudo touch /etc/containers/nodocker
# Docker (Optional)
#sudo apt install docker.io

# Optional dependcies for minor features
sudo apt install -y systemd-container
```

## Cloning the repository

```
git clone --recurse-submodules https://github.com/UtsavBalar1231/bsp.git -b master

```

## Build
```
cd bsp
./bsp <soc> (e.g., ./bsp rk356x)
```
