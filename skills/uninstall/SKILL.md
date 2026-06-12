---
description: Completely remove the wait.money client, its status line hook, and local config from this machine.
disable-model-invocation: true
---

Uninstall the wait.money client.

1. Confirm with the user that they want to remove wait.money from this machine. Unredeemed linked earnings stay attached to their account server-side; anonymous device earnings are abandoned.
2. Run `waitmoney uninstall`. It removes the status line hook, the spinner config, the installed scripts, and the PATH symlink.
3. Show the user the output and confirm removal. The change takes effect in new Claude Code sessions.
