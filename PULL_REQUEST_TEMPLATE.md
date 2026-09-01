<!--
Thanks for contributing to astro-game-lab! Please fill in the sections below.
For small changes (typo fixes, etc.) feel free to keep this brief.
-->

## Summary

<!-- What does this PR do, and why? One or two sentences is usually enough. -->

## Related issues

<!-- Link any related issues. Use "Fixes #123" to auto-close an issue on merge, or "Refs #123" for a softer link. -->

## Type of change

<!-- Check all that apply. -->

- [ ] Bug fix (non-breaking change that fixes an issue)
- [ ] New feature (non-breaking change that adds functionality)
- [ ] Breaking change (fix or feature that changes existing behavior)
- [ ] Physics / simulation change
- [ ] Game design, balance, or content change
- [ ] Art, audio, or other assets
- [ ] Documentation update
- [ ] Refactor / internal cleanup
- [ ] Test-only change
- [ ] Build / CI / tooling change

## How has this been tested?

<!-- Describe the tests you ran and how a reviewer can reproduce them. For gameplay changes, say what you played and what you saw. -->

## Physics changes

<!-- Delete this section if your PR does not touch simulation or physics code. -->

- **Units and frame:** <!-- e.g. SI, ECI (J2000) -->
- **Reference / source:** <!-- textbook, paper, standard, with equation number where possible -->
- **Validated against:** <!-- published worked example, GMAT, poliastro/astropy, JPL Horizons, closed-form solution -->
- **Assumptions and domain of validity:** <!-- what is neglected, and where the model stops being valid -->
- [ ] Added or updated a validation test with the expected values and their source.
- [ ] Checked the edge cases (circular, equatorial, hyperbolic, near-parabolic) that apply.
- [ ] No gameplay simplifications were added to the physics core.

## Determinism

<!-- Delete this section if your PR does not touch simulation state. -->

- [ ] No unseeded randomness; simulation uses the repo's seeded RNG.
- [ ] No wall-clock reads inside the simulation.
- [ ] Existing replays and saved scenarios still reproduce, or the migration is described above.

## Assets

<!-- Delete this section if your PR adds no art, audio, models, or data. -->

- [ ] I created these assets, or they are under a licence compatible with this repository.
- [ ] Sources and licences are recorded in the repo's attribution file.
- [ ] Large binaries are handled per the repo's convention (LFS, download script, or external host) rather than committed raw.

## Checklist

- [ ] I have read the [Contributing Guide](https://github.com/astro-game-lab/.github/blob/main/CONTRIBUTING.md).
- [ ] My change follows the repository's style and conventions.
- [ ] I have added tests that prove my change works, or explained why none are needed.
- [ ] New and existing tests pass locally.
- [ ] I have updated the documentation where relevant.
- [ ] The PR title is clear and descriptive.

## Additional notes

<!-- Anything reviewers should pay special attention to? Known limitations? Follow-ups? Screenshots or a clip are very welcome for visual changes. -->
