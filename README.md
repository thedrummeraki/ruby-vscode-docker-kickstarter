# Akinyele's Ruby VSCode kickstarter

This repository houses set up needed to start any Ruby project running on Docker to be used with Visual Studio Code.

## Requirements

- VS Code (with [Dev Containers](https://marketplace.visualstudio.com/items?itemName=ms-vscode-remote.remote-containers) extension installed)
- Docker
- Love for Ruby :D

## Usage

Cloning this repo gives you:
- A Docker Compose config file
- Dev Container configs with some extensions preinstalled, including but not limited to:
  - Ruby LSP
  - Solargraph
  - pry

There is no need to build the image locally. The image is already prebuilt and can be fetched as follows:

```bash
docker pull drummeraki/ruby-kickstarter:3.3.3
```

> Note: A label must be specified. I don't use `latest` with those images.
