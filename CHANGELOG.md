# Changelog

## Unreleased

- Agents can mark a task as human over MCP, and a Human only switch next to New task (toggled with `h`) filters the board to those tasks. Thanks @eniewold.
- `--listen <ADDR>` sets the address the board listens on for one run, like `--port`.
- `Dockerfile` and `compose.yaml` run one board in a container on a server; agents connect over HTTP MCP.
