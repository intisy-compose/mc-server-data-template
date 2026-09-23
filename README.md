# mc-server-data-template

Public default Minecraft server data for game-compose.

Default data for the `mc` slot of
[game-compose](https://github.com/intisy-compose/game-compose), so a fresh
`git clone --recursive` runs out of the box. It holds no server files yet: the server image
generates its defaults on first start, and runtime state (worlds, saves, logs) is gitignored.

## Use your own data

Fork or replace this repo and commit your configuration (`server.properties`, `bukkit.yml`, `config/` and plugin configs), then point the slot at it
from the game-compose checkout:

```powershell
.\docker-compose.ps1 data use mc <owner/repo[@ref]>   # your own data repo, optionally a branch
.\docker-compose.ps1 data use mc                      # back to this template
```

Commit configuration, not runtime state.

## License

[![MIT License](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)
