---
description: Link this device's wait.money earnings to the user's Google account so the balance is theirs across devices. Runs waitmoney login and walks the user through approving the short code in the browser.
---

Link the user's wait.money device to their account.

1. Run `waitmoney login`. It prints a short code (like `ADX-XXXXX`) and a verify URL.
2. Tell the user: open the verify URL in a browser, sign in with Google, type the code, confirm the request details (IP and location shown on the page must be theirs), and click approve.
3. `waitmoney login` polls and confirms in the terminal once linked. Report the linked email back to the user.
4. If `waitmoney` is not on PATH, the client is not installed; point the user to `/wait-money:install`.
