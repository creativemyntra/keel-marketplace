# Keel Marketplace

Claude Code plugin marketplace for [Keel](https://github.com/<org>/keel).

## Install Keel

In Claude Code (terminal) or Claude Desktop:

```
/plugin marketplace add <org>/keel-marketplace
/plugin install keel@keel-marketplace
```

Then, one time in your project repo, run the setup wizard to create your state files:

```bash
bash setup.sh
```

The plugin ships the engine (agents, commands, hooks, MCP). The wizard creates the per-repo state/memory/decision files, which by design live in your repo and are git-committed — they can't ship inside a cached plugin.
