---
description: Install the wait.money client. A signed one-line installer adds a sponsored line to the Claude Code status line and starts accruing earnings. macOS, Linux, and Windows (beta), Node 18+.
disable-model-invocation: true
---

Install the wait.money client for the user.

1. Run the signed installer (ed25519 signature + per-file sha256 verification happen inside the script).

   macOS / Linux:

   ```bash
   curl -fsSL https://wait.money/install.sh | sh
   ```

   Windows (beta, PowerShell):

   ```powershell
   irm https://wait.money/install.ps1 | iex
   ```

2. Show the user the installer output. On success, tell them:
   - The sponsored status line activates in new Claude Code sessions. It shows one ad line plus a live earnings ticker.
   - Earnings accrue anonymously to this device right away. To attach them to an account, run `/wait-money:link`.
   - `waitmoney pause` and `waitmoney resume` toggle the ad line. `/wait-money:uninstall` removes everything.
   - Privacy: no prompts, code, file paths, or AI responses are ever collected. Details: https://wait.money/privacy

3. If the installer reports Node older than 18, tell the user to upgrade Node and retry. Do not work around the requirement. On Windows, remind the user the support is beta and a new terminal is needed after install (the PATH update applies to new shells).
