# Rust Dev Environment

## Prerequisites

- [Docker](https://docs.docker.com/get-docker/) or [Podman](https://podman.io/getting-started/installation)
- [DevPod](https://devpod.dev/docs/installation)

## Start the dev environment with

```bash
devpod up . --dotfiles https://github.com/froko/dotfiles-devcontainer.git
```

## Troubleshooting

You may experience an issue with lazy-lua showing no or just a few files.
This is a known issue on macOS and can be fixed by running the following
commands in the DevContainer terminal:

```bash
sudo rm /usr/local.bin/fd
sudo rm /usr/local.bin/rg
sudo apt update
sudo apt install fd-find ripgrep
```

## References

- [dotfiles-devcontainer](https://github.com/froko/dotfiles-devcontainer)
