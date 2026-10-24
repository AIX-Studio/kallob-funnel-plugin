# Kallob Funnel 1.0.0

Kallob Funnel for Codex: sales funnels for your shop, written by Codex on your own machine and run from your own Cloudflare. Your work stays on this machine; your Kallob account decides whether Kallob Funnel is open after you sign in.

## Install

```bash
codex plugin marketplace add AIX-Studio/kallob-funnel-plugin
codex plugin add kallob-funnel@kallob-funnel
```

Quit and reopen Codex, then ask it to "open Kallob Funnel". Kallob Funnel needs Node.js 22.5 or newer; Codex offers to install it when it is missing. In Kallob Funnel, open Settings → Connect Kallob.

Kallob Funnel updates itself from Kallob Cloud. Your data lives in `~/.kallob-funnel`.

Package 1.0.0, seed Studio 1.0.0 (7ef62c4-mvlynafx), built from `7ef62c4` of the private kallob-funnel-studio repository by `scripts/release-plugin.mjs`. Do not edit this repository by hand.
