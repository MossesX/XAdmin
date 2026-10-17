# XAdmin

Administration and developer panels for AmberX (from the README).

## Status (as of Oct 17 2026)

- **Empty so far:** the repo holds only a README and no code yet.
- **Possible overlap:** the AmberX AXF framework already plans `lib-admin` (a placeholder module) and has a web Dev Console in `MossesX/AmberX-AXF` (`apps/console-web`). Before building here, ask Brett whether XAdmin is still a separate project or folds into those.

## Related repos

- `MossesX/AmberX-AXF`: the framework, Dev Console and `lib-admin`.
- `MossesX/axHub`: connector hub. Its admin API is meant to be managed from AXF consoles.

## Working with Brett (same in every MossesX repo)

- **Where he works:** mostly from his Android phone (Samsung Galaxy S26 Ultra), often through **Moshi** (mosh) into his Hostinger VPS, where Claude Code runs. Keep replies phone-readable: lead with the result, short paragraphs, no walls of text.
- **Model choice:** before any build task, recommend which model to use and why, then let him pick from the top three (Fable, Opus, Sonnet). Use Fable where it's warranted, Opus for most work, and Sonnet only when you're sure Opus isn't needed.
- **The repo is the shared memory.** Sessions on the phone (Moshi), desktop, web and claude.ai don't share chat history, so anything a future session needs must live in this repo. Commit and push often with clear messages, and update the **Status** section of this file whenever something meaningful changes.
- **No secrets in the repo:** no tokens, passwords, keys or IPs with credentials. Use environment variables or GitHub Actions secrets.
- **GitHub:** account `MossesX`. A new repo must exist on GitHub before a session can push to it.
- **Server:** a Hostinger VPS running **Coolify**. Coolify's Traefik proxy owns ports 80/443, so new web apps go behind it as Coolify apps (no separate nginx). His domain is `amberxai.com`.
- **axHub:** his connector hub on the VPS (repo `MossesX/axHub`). If the axHub MCP server is configured in this Claude Code install, use its `list_services`, `describe_service` and `call` tools to reach his other services instead of asking him for credentials.
