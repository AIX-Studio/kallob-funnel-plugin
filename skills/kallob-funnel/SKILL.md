---
name: kallob-funnel
description: Open Kallob Funnel (funnels, leads, orders, products, payment and delivery, my shop, putting funnels online, settings) with funnel_studio_open, or work on a task Kallob Funnel hands to Codex. Use for Kallob Funnel.
---

# Kallob Funnel

Kallob Funnel runs on this machine: the founder makes sales funnels, Codex writes their pages, and the funnels go online on the founder's own Cloudflare. When Kallob Funnel hands Codex a task, its prompt says what to do, how, its limits and where the result goes; follow it. Do not bring in other installed skills or playbooks for a Kallob Funnel task.

## First run: Node.js

Kallob Funnel runs on this machine with Node.js 22.5 or newer. If the `kallob-funnel` MCP tools are missing, or calling one fails because the server cannot start, check before anything else:

1. Run `node --version`. If it prints `v22.5.0` or newer, Node is not the problem: report the tool's error instead.
2. Otherwise install the current Node.js LTS, telling the person what you install and why:
   - macOS: `brew install node` when Homebrew is installed; otherwise download the macOS installer (.pkg) from https://nodejs.org/en/download and ask the person to run it.
   - Windows: `winget install --id OpenJS.NodeJS.LTS -e`.
3. Run `node --version` again, then ask the person to quit and reopen Codex so the plugin starts with Node. Do not continue with the request until the tools are available.

## Updates

Kallob Funnel updates itself from Kallob Cloud. If a tool answers that Kallob Funnel is updating, wait about a minute and call it again; do not work around it.

## Open Kallob Funnel

When the person wants to see or work in Kallob Funnel, call `funnel_studio_open` from the `kallob-funnel` MCP server (optionally with `section`: `funnels`, `leads`, `orders`, `products`, `payment`, `shop`, `online` or `settings`) and open the returned `url` in the in-app browser. It starts Kallob Funnel when needed; the person's data stays on this machine.

If a tool says Kallob is not connected, call `funnel_studio_open` with `section: "settings"`, open the url, and ask the person to click Connect Kallob, then continue.

Keep the following behind explicit authorization: publishing, sending, spending, commitments and other consequential actions.
