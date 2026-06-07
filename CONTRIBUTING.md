# Contributing to KTCEDC

Policy:
- All changes must be made via Pull Request and require at least one approving review from a CODEOWNER (@KantaponM or @RepoKan).
- Direct pushes to protected branches are forbidden for everyone except @KantaponM and @RepoKan.
- Use topic branches named `yourname/feature/short-desc`.

Commit messages:
- Follow Conventional Commits style: `type(scope): short summary`.
  - Example: `feat(login): add biometric fallback`

Pull requests:
- Include a description, linked issues, and tests where appropriate.
- Ensure CI passes before merging.

Code reviews:
- At least one approving review by a code owner is required.
- Large or security-sensitive changes should request additional maintainer review.

Testing:
- Add unit tests for new logic.
- Include test instructions in PRs and ensure CI passes.

Release & backups:
- Tag releases following semantic versioning when appropriate.
- Store backup artifacts under `backups/` and document recovery steps in `docs/recovery.md`.
