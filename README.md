# wait.money plugin for Claude Code

Earn from your terminal. wait.money puts one sponsored line in your Claude Code status line (with a live earnings ticker) and pays you a share of cleared ad revenue. macOS, Linux, and Windows (beta), Node 18+.

## Install

In Claude Code:

```
/plugin marketplace add kairothq/wait-money-plugin
/plugin install wait-money@wait-money
/wait-money:install
```

The installer is signed (ed25519) with per-file sha256 verification, and the client self-updates with monotonic version checks.

## Commands

| Command | What it does |
|---|---|
| `/wait-money:install` | One-line signed install of the client |
| `/wait-money:link` | Link this device's earnings to your Google account |
| `/wait-money:status` | Version, paused/active, linked account, balance |
| `/wait-money:uninstall` | Remove everything from this machine |

The installed `waitmoney` CLI also works directly: `waitmoney status | pause | resume | spinner | uninstall`.

## Privacy

wait.money never collects prompts, source code, file paths, or AI responses. The event schema cannot carry them. Full policy: https://wait.money/privacy

## Notes

- This plugin is a thin wrapper over the same signed installer served at the site. Installing via `curl` directly is equivalent.
- Works in any terminal Claude Code runs in, including the Zed and Cursor terminals.
