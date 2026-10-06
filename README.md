# Wikipedia Discord bot

An earlier JavaScript bot that responds to `wiki` commands with Wikipedia article links in French or English.

```text
wiki en Apple
wiki fr Pomme
```

## Setup

Create your own bot in the [Discord developer portal](https://discord.com/developers/applications), invite it to your server, then install dependencies locally:

```sh
npm ci --ignore-scripts
```

Set `DISCORD_BOT_TOKEN` through your shell or secret manager, then run `node index.js`. Never commit the token. Installed `node_modules` are excluded from version control; the manifest and lock file describe dependencies.

## Compatibility

This project still uses discord.js 12 and legacy collection APIs. A migration to a supported discord.js version, intents configuration, and live bot testing are required before relying on it. No Discord connection or message delivery is part of the local syntax check:

```sh
node --check index.js
```

See [SECURITY.md](SECURITY.md) for private vulnerability reports.
