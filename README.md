# Open Video

Cursor plugin for the [Open Video](https://open.video) publisher platform. Connects to the hosted MCP at `https://mcp.open.video/mcp` (remote HTTP — required for Grok Bot).

Catalog display name: **Open Video**. Identifier: `open-video`.

## Install from Cursor Marketplace

Search **Open Video** in [Cursor Marketplace](https://cursor.com/marketplace) and in Grok Bot → Plugins (same catalog). Sign in when Cursor prompts (Open Video OAuth). This package has **no API key**. Auth is the hosted MCP OAuth flow, not a secret in `mcp.json`.

Not the Grok Build marketplace (`github.com/xai-org/plugin-marketplace`).

## Local install

Use this when developing the listing package, or before the Marketplace listing is live.

1. Copy this folder to `~/.cursor/plugins/local/open-video`, or clone it there.
2. In Cursor: Command Palette → **Developer: Reload Window** (IDE). Cursor Agent CLI: enable the local plugin in the session.
3. Sign in when prompted.
4. One successful tool call (for example listing channels) confirms it works.

## What the plugin can do

The remote server at `https://mcp.open.video/mcp` exposes Open Video publisher tools (account, channels, videos, playlists, monetization, and related APIs). It does not add Cursor filesystem or shell tools. Installing it means you trust that hosted endpoint the same way you trust signing into open.video.

## Assets

| File | Use |
|------|-----|
| `assets/plugin-logo.png` | Catalog tile. Official Open Video 512×512. Referenced by `.cursor-plugin/plugin.json` `logo` (path is from the **plugin root**, not from `.cursor-plugin/`). |
| `assets/logo.png` | Wide wordmark (524×266). Kept; not the catalog `logo` field. |

## License

MIT. See `LICENSE`.
