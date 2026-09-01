# Contributing to astro-game-lab

Thanks for your interest in contributing! This document explains how to get involved across the astro-game-lab organization. Individual repositories may provide their own `CONTRIBUTING.md` that overrides or extends these defaults.

## Before you start

- Read the [Code of Conduct](CODE_OF_CONDUCT.md). Participation in astro-game-lab is governed by it.
- Check the repo's open issues and discussions. Someone may already be working on what you have in mind.
- For anything larger than a small fix, **open an issue first** so we can align on approach before you invest time.

## Ways to contribute

- **Report bugs** — open an issue using the bug report template with steps to reproduce.
- **Report wrong physics** — if the simulation disagrees with reality, use the **physics discrepancy** template. These are our highest-priority bugs.
- **Suggest features, mechanics, or scenarios** — open an issue using the feature request template.
- **Playtest** — tell us where a game is confusing, unfair, boring, or unexpectedly great. Playtest reports are genuinely useful.
- **Improve documentation** — typo fixes, clarifications, and new examples are always welcome.
- **Submit code** — fix bugs, implement features, add tests, or improve performance.
- **Contribute art, sound, or scenario design** — see [Assets and licensing](#assets-and-licensing) before you do.
- **Answer questions** — help others in [Discussions](https://github.com/orgs/astro-game-lab/discussions).
- **Review pull requests** — thoughtful review from the community is highly valued.

## Development workflow

1. **Fork** the repository and clone your fork.
2. **Create a branch** with a short, descriptive name (e.g. `fix-lambert-multirev`, `add-porkchop-view`).
3. **Make your changes.** Keep commits focused and the diff minimal.
4. **Add tests** where applicable. If a repo has a test suite, your changes should pass it.
5. **Run linters/formatters** configured by the repo before committing.
6. **Push** to your fork and **open a pull request** against the default branch.
7. Fill in the pull request template. Link related issues with `Fixes #123` or `Refs #123`.

## Physics and simulation changes

These carry extra requirements, because the honesty of the simulation is the point of the organization.

- **State your units and reference frame.** Every function that takes or returns a physical quantity should say which. SI (metres, seconds, kilograms, radians) is the default everywhere inside a physics core.
- **Cite your source.** Link the textbook, paper, or standard the algorithm comes from — author and equation number where you can.
- **Include a validation test.** Compare against an independent reference: a published worked example, GMAT, `astropy`/`poliastro`, JPL Horizons, or a closed-form solution. Put the expected values and their source in the test.
- **Say what you are neglecting.** J2 only? Two-body? Spherical Earth? Document the model's domain of validity and where it breaks down.
- **Keep gameplay cheats out of the core.** Simplifications that exist to make the game fun belong in the game layer, clearly labelled, never silently baked into the physics.
- **Watch the singularities.** Circular and equatorial orbits, hyperbolic cases, and near-parabolic transfers are where these algorithms break. Test them.

## Determinism

Anything that touches simulation state must be deterministic — replays, shared scenarios, and reproducible bug reports all depend on it.

- Use the repo's seeded RNG. Never `Math.random()`, `random.random()`, or an unseeded generator in simulation code.
- Never read the wall clock inside the simulation. Physics runs on a fixed timestep, decoupled from rendering.
- Avoid iteration over unordered containers where the order affects results.

## Commit messages

- Use the imperative mood in the subject line: "Add Lambert solver" rather than "Added" or "Adds".
- Keep the subject under 72 characters.
- Use the body to explain *why* the change is being made when it is not obvious.
- Reference issues (`Fixes #123`) where applicable.

## Pull request review

- A maintainer will review your PR as soon as possible. Please be patient — we are a volunteer community.
- Expect feedback. Reviews are a conversation; changes requested are not a judgment of you or your work.
- Keep PRs focused. Unrelated changes belong in separate PRs.
- Keep your branch up to date with the base branch, using rebase or merge per the repo's convention.

## Assets and licensing

Unless a repository states otherwise, astro-game-lab code is released under the **MIT License**, and game assets (art, audio, models, scenario content) under **CC BY 4.0**. Each repo states its own terms in its `LICENSE` file — check before contributing.

By contributing, you agree that your contributions are licensed under the same terms as the repository you contribute to.

**Only contribute assets and data you have the right to license this way.** That means:

- No AI-generated assets whose training data or output licensing you cannot vouch for.
- No ripped, traced, or derived assets from commercial games, films, or stock libraries.
- Attribute any third-party material and confirm its licence is compatible. Record it in the repo's attribution file.
- Ephemeris data, SPICE kernels, TLEs, and imagery all have terms — check them, cite the source, and prefer linking or a download script over committing large binaries.

## Questions?

Open a thread in [GitHub Discussions](https://github.com/orgs/astro-game-lab/discussions) or ask in the relevant repository's issue tracker.
