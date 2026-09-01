# Governance

This document describes how the astro-game-lab organization is run. It is intentionally lightweight and will evolve as the community grows.

## Mission

astro-game-lab develops open-source games built on real astrodynamics. We aim to make orbital mechanics something people can learn by playing, and to leave behind reusable, honest simulation code that others can build on.

## Roles

### Players

Anyone who plays an astro-game-lab game. Players are encouraged to report bugs, share playtest feedback, ask questions, and suggest improvements.

### Contributors

Anyone who contributes — via code, physics review, documentation, art, audio, scenario design, playtesting, or other means. There is no formal application: open a pull request, file a good bug report, or help answer a question and you are a contributor.

### Maintainers

Contributors with commit rights on one or more repositories. Maintainers are responsible for:

- Reviewing and merging pull requests.
- Triaging issues.
- Guiding the technical and design direction of their repository.
- Upholding the [Code of Conduct](CODE_OF_CONDUCT.md).

New maintainers are invited by existing maintainers based on sustained, high-quality contribution and good judgment. There is no fixed threshold; invitation is by consensus of the current maintainers of the repository in question.

### Organization administrators

A small number of individuals have administrative rights over the GitHub organization itself (creating repositories, managing teams, etc.). Admins act on behalf of the community and follow the same decision-making processes as maintainers.

## Decision making

We aim for **lazy consensus**: proposals are assumed to have support unless someone objects. For most decisions, a discussion on the relevant issue or pull request is sufficient.

For decisions that affect multiple repositories or the organization as a whole (e.g. adopting a new game, changing organization-wide policies), an RFC-style discussion in [Discussions](https://github.com/orgs/astro-game-lab/discussions) is the norm. Anyone may open one; resolution is by rough consensus among active maintainers.

If consensus cannot be reached, organization administrators may make a final call, with reasoning recorded in the discussion.

## Design decisions

Games are opinionated in a way that libraries are not, and design disagreements are not settled by correctness alone.

- **Physics correctness is not a matter of consensus.** If the simulation disagrees with reality, that is a bug, and reference data wins the argument.
- **Design and fun are matters of judgment.** Where a change trades fidelity for playability, the repository's maintainers decide, and the reasoning is recorded in the issue or PR.
- **Each game has a design lead** — usually its originating maintainer — who holds the final say on that game's direction. This keeps games coherent rather than designed by committee.

## Adding a new repository

New repositories join the organization when:

1. They fit the organization's mission.
2. There is at least one willing maintainer.
3. They adopt the default community health files and a `LICENSE` (or equivalents).

Proposals for new repositories should be opened as a Discussion before the repository is created.

## Archiving or removing a repository

Repositories that become unmaintained may be archived. A game that is finished is not unmaintained — "done" is a legitimate end state, and archiving one is a normal outcome rather than a failure. Removal is reserved for exceptional cases (e.g. legal or licensing issues). Either action is discussed publicly before being taken.

## Changes to this document

This document can be changed by opening a pull request. Material changes should have broad discussion before merging.
