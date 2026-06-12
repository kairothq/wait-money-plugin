# Adline plugin for Claude Code

Earn from your terminal. Adline puts one sponsored line in your Claude Code status line (with a live earnings ticker) and pays you a share of cleared ad revenue. macOS and Linux, Node 18+.

## Install

In Claude Code:

```
/plugin marketplace add kairothq/adline-plugin
/plugin install adline@adline
/adline:install
```

The installer is signed (ed25519) with per-file sha256 verification, and the client self-updates with monotonic version checks.

## Commands

| Command | What it does |
|---|---|
| `/adline:install` | One-line signed install of the client |
| `/adline:link` | Link this device's earnings to your Google account |
| `/adline:status` | Version, paused/active, linked account, balance |
| `/adline:uninstall` | Remove everything from this machine |

The installed `adline` CLI also works directly: `adline status | pause | resume | spinner | uninstall`.

## Privacy

Adline never collects prompts, source code, file paths, or AI responses. The event schema cannot carry them. Full policy: https://adline-divys-projects-a4af20de.vercel.app/privacy

## Notes

- This plugin is a thin wrapper over the same signed installer served at the site. Installing via `curl` directly is equivalent.
- Works in any terminal Claude Code runs in, including the Zed and Cursor terminals.
