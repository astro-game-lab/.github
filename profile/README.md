# astro-game-lab

Open-source astrodynamics and space games. Real orbital mechanics, playable.

## What is astro-game-lab?

**astro-game-lab** builds games where the space is not set dressing. Orbits are propagated, not animated along a spline; transfers cost the delta-v they actually cost; a rendezvous is hard for the same reasons it is hard in real life.

We think orbital mechanics is one of the most beautiful and least intuitive things a person can learn, and that a game is the best teacher it will ever get. So we make the simulation honest, and then we make it fun.

## Core focus areas

- **Playable astrodynamics** — two-body and patched-conic games, transfer and rendezvous puzzles, station-keeping and constellation management, launch windows and porkchop plots you can actually fly.
- **Honest physics cores** — propagators, force models, coordinate and time systems, written to be verifiable against reference data and reusable across games.
- **Space operations** — mission planning, ground station scheduling, conjunction assessment, and the debris environment, as game mechanics.
- **Learning through play** — scenarios that teach a concept by making you use it, with the real numbers visible when you want them.
- **Reusable pieces** — engines, solvers, and rendering components that other people can build their own space games on.

## Design principles

1. **The simulation tells the truth.** The physics core is validated against reference data. Where a game layer simplifies or cheats for playability, it is documented and separable — never smuggled into the core.
2. **Real units, real numbers.** SI internally, always. A player who looks up the delta-v for a Hohmann transfer to GEO should find the game agrees.
3. **Deterministic and reproducible.** Same seed and same inputs give the same run, on every platform. Replays and shared scenarios depend on it.
4. **Playable first.** Fidelity is a means, not the goal. If a model is more accurate but makes the game worse to play, it goes behind a toggle.
5. **Open all the way down.** Permissive licenses, open formats, no assets or data we cannot redistribute.

## Repositories

The organization is just getting started — the first repositories are on their way. Watch this space, or open a [Discussion](https://github.com/orgs/astro-game-lab/discussions) if you want to help shape what comes first.

## How to contribute

We welcome contributions of all sizes, and not only code.

1. **Browse the repositories** and find something that interests you.
2. **Check the issues** on the relevant repo — look for `good first issue` or `help wanted` labels.
3. **Open an issue** before large changes so we can align on approach.
4. **Fork, branch, and open a pull request.** Follow the repo's `CONTRIBUTING.md` if present.
5. **Join the discussion** — ideas, questions, playtest feedback, and bug reports are all valuable.

Game development needs more than programmers. Art, sound, level and scenario design, UX, writing, accessibility work, and playtesting are all real contributions here.

See [CONTRIBUTING.md](https://github.com/astro-game-lab/.github/blob/main/CONTRIBUTING.md) for the details.

## Discussions

Have a question, an idea, or a game concept to pitch? Join us in [GitHub Discussions](https://github.com/orgs/astro-game-lab/discussions).
