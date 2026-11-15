# MangaBaaz Instagram Publisher plugin

Connects your AI app to [MangaBaaz](https://mangabaaz.vercel.app), a remote MCP server that publishes images, carousels, Reels and Stories to an Instagram Business or Creator account.

No API key, environment variable or Authorization header is needed. On first use your app registers itself, opens the MangaBaaz consent page and stores its own OAuth credentials. You sign in with your Instagram account and approve access. Instagram credentials stay on the server, and each user only reaches their own accounts.

MangaBaaz is invite-only. [Request access](https://mangabaaz.vercel.app/request-access) first.

## Install

Claude Code:

```bash
/plugin install mangabaaz --marketplace sadeghianme/mangabaaz-plugin
```

Then run `/mcp` and sign in to the `mangabaaz` server.

Any MCP client (Claude, Codex, others) can instead add the server URL as a custom connector:

```
https://mangabaaz.vercel.app/api/mcp
```

Step-by-step instructions for each app: <https://mangabaaz.vercel.app/setup>

## Contents

| File | Purpose |
| :- | :- |
| `.claude-plugin/plugin.json` | Claude plugin manifest |
| `.claude-plugin/marketplace.json` | Lets Claude Code install this repo directly |
| `.mcp.json` | Remote Streamable HTTP MCP server definition |
| `plugin.json`, `mcp.json` | Portable manifest with Codex interface metadata |
| `assets/logo.png` | Listing logo |

Privacy policy: <https://mangabaaz.vercel.app/privacy>. Licensed under MIT.
