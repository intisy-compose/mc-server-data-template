# Minecraft server data (template)

Public **template** data repo for [game-compose](https://github.com/intisy-compose/game-compose).
It is the default mounted into the `mc-server-data-template` slot so a fresh clone runs out of the box.

Holds a Paper/Spigot server configuration: `server.properties`, plugin configs, and similar. Actual worlds and logs are runtime state and are ignored.

## Use your own data

Fork or replace this repo, then point the slot at it:

```bash
./data.sh use mc-server <owner/repo[@ref]>   # from the game-compose repo
```

Worlds, saves and logs are gitignored — commit configuration, not runtime state.

## License

MIT
