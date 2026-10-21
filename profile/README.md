<div align="center">

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/naulonapp/.github/main/profile/assets/naulon-lockup-dark.png">
  <img src="https://raw.githubusercontent.com/naulonapp/.github/main/profile/assets/naulon-lockup-light.png" alt="naulon" height="64">
</picture>

### Humans read free. Machines pay.

[Website](https://naulon.app) · [Docs](https://naulonapp.github.io/naulon/) · [Blog](https://naulon.app/blog) · [Changelog](https://naulon.app/changelog)

</div>

A toll you put in front of a site. AI agents and crawlers pay a fraction of a cent in USDC to
read or cite a page, it settles straight to the author's own wallet, and people read free.

Language models read writing at scale and pay nothing for it. naulon changes that one exchange:
a human request passes through untouched, a machine request gets `402 Payment Required` and
pays before it reads. The fare is the *naulon*, the old coin you paid to cross.

### Repositories

| | |
|---|---|
| **[naulon](https://github.com/naulonapp/naulon)** | The gate and its console, the in-app toll, the WordPress plugin and the paying agent. MIT. |
| **[naulon-plugins](https://github.com/naulonapp/naulon-plugins)** | The plugin for ChatGPT/Codex and Claude Code: pay for and cite tolled sources. |

### Start

```bash
curl -O https://raw.githubusercontent.com/naulonapp/naulon/main/docker-compose.yml
npx -p @naulon/sdk naulon init   # writes .env and config/credits.json
docker compose up -d             # gate on :8402, console on :8403
```

Or skip hosting: [naulon.app](https://naulon.app) runs the gate for you, with the same protocol
and the same custody-free settlement. Built on Circle's nanopayment rail, Arc-first, over HTTP 402.
