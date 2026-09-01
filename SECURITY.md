# Security Policy

The astro-game-lab community takes the security of its software seriously. Thank you for helping us keep our players and contributors safe.

## Supported versions

Individual repositories declare their own support policy. Unless otherwise stated in a repository's own `SECURITY.md`, only the latest released version of each project receives fixes.

## Reporting a vulnerability

**Please do not report security issues through public GitHub issues, discussions, or pull requests.**

Instead, report them privately using GitHub's [private vulnerability reporting](https://github.com/astro-game-lab/.github/security/advisories/new) on the affected repository (or on this `.github` repository if you are unsure which repo is affected).

When reporting, please include as much of the following as you can:

- The repository and version affected.
- A description of the issue and its impact.
- Steps to reproduce, or a proof-of-concept if available.
- Any known mitigations or workarounds.
- Whether you plan to publicly disclose and, if so, your preferred timeline.

## What to expect

- We will acknowledge receipt of your report within **5 business days**.
- We will provide an initial assessment within **10 business days**.
- We will keep you informed of progress toward a fix and coordinate a disclosure timeline with you.
- We will credit you in the advisory once the issue is resolved, unless you prefer to remain anonymous.

## Scope

This policy covers source code and published artifacts of repositories within the [`astro-game-lab`](https://github.com/astro-game-lab) GitHub organization.

Areas we care about particularly, given what we build:

- **Untrusted content.** Save files, replays, scenario and mod files, and level definitions are attacker-controlled input. Deserialization flaws, path traversal on load, and code execution through a scenario script are in scope.
- **Multiplayer and networking.** Anything in a client or server that lets a peer crash, hang, or execute code on another player's machine.
- **Web builds.** XSS and similar issues in browser-hosted games and their surrounding pages.
- **Supply chain.** Compromised or typosquatted dependencies, and malicious content in asset pipelines.

Out of scope:

- Vulnerabilities in third-party dependencies (please report those to the respective projects; we welcome notifications so we can upgrade).
- Issues affecting only unsupported versions.
- Findings from automated scanners without a demonstrable impact.
- **Game cheating in single-player.** Editing your own save or memory to get infinite delta-v is not a vulnerability. Cheating that affects *other players* in a multiplayer or shared-leaderboard context is.

## Safe harbor

We support good-faith security research. If you follow this policy when reporting a vulnerability to us, we will:

- Consider your research authorized and will not pursue or support legal action against you.
- Work with you to understand and resolve the issue promptly.

Thank you for helping keep astro-game-lab and its players safe.
