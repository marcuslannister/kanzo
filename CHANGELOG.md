# Changelog

## Unreleased

- Windows (x64): a PowerShell installer or a zip, `kanzo service install` as a Task Scheduler task with no window, and updates from the board or `kanzo update`.
- Agents can mark a task as human over MCP, and a Human only switch next to New task (toggled with `h`) filters the board to those tasks. Thanks @eniewold.
- `--listen <ADDR>` sets the address the board listens on for one run, like `--port`.
- `Dockerfile` and `compose.yaml` run one board in a container on a server; agents connect over HTTP MCP (`claude mcp add --transport http …`).
- The Docker board syncs with a private repo over HTTPS: a fine-grained token in `secrets/git-credentials`, mounted read-only. The README has the token steps and the usual errors.
