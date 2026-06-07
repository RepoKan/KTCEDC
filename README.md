# KTCEDC

KTCEDC is an Android application project focused on behavior-driven features, maintainability (MA-style modular code), and resilient backups for code recovery. This repository provides guidelines, tooling, and examples to help contributors implement features with secure review and recovery workflows.

## Purpose

- Implement Android app features where "behavior files" describe expected behaviors and guide development.
- Organize code for maintainability and ease of review.
- Provide backup/restore approaches and documentation to recover code if needed.
- Enforce security and code-review controls to protect the source and team activity.

## Getting started (developer)

1. Install Android Studio and the Java/Kotlin toolchain (JDK 11+ recommended).
2. Clone the repository:
   git clone https://github.com/RepoKan/KTCEDC.git
3. Open the project in Android Studio and use Gradle to build and run the app.

## Project layout (recommended)

- app/ - Android app module (source code, resources)
- behavior/ - behavior specification files (human-readable YAML/JSON that describe feature behavior)
- docs/ - architecture notes, recovery instructions, onboarding
- backups/ - automated or manual backup artifacts (encrypted archives, diffs)

## Development workflow

- Create topic branches: `git checkout -b <yourname>/feature/short-desc`
- Keep commits small and focused; use conventional commit messages.
- Open a Pull Request targeting `main` and request at least one review using the CODEOWNERS file.
- CI runs on PRs and must pass before merging.

## Copilot Spaces

This repo includes example configuration to help you use GitHub Copilot Spaces. See `.copilot/example-space.md` for recommended Space contents and instructions. Use the provided `mcp_config.json` to enable the `copilot_spaces` toolset in your MCP client.

## Security & backups

- Do not commit secrets or credentials. Use encrypted secrets or a secure secret manager for CI.
- Follow the instructions in SECURITY.md to report vulnerabilities.
- Store backups in `backups/` and ensure sensitive backups are encrypted.

For more information about contributing and code reviews, see CONTRIBUTING.md and CODE_OF_CONDUCT.md.
