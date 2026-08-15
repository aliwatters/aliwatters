# What aliwatters is for

**This repository supplies the README that GitHub renders as the `aliwatters` account profile.**

## Why this document exists

This settles whether `aliwatters/aliwatters` is an application repository or an account-profile surface. The committed guidance identifies it as GitHub's special profile README repository, and the tracked tree contains only profile documentation. Its purpose is therefore to control the profile README, not to host executable software.

## What it does

- Keeps the public profile content in the top-level `README.md`.
- Uses the GitHub profile-repository marker in `README.md`, which names `aliwatters/aliwatters` as the special repository whose README appears on the account profile.
- Records the handling boundary in `CLAUDE.md`: edits to `README.md` are publicly visible on the GitHub profile, while `rod-mcp.yaml` is untracked local tooling configuration.

## What it is not for

- It is not an executable application or service: the tracked tree has no source directory, executable entry point, or command definition.
- It is not a package or library: there is no package manifest, exported implementation, or distribution configuration.
- It is not a test, CI, or deployment project: the tracked tree has no test files, workflow definitions, or deployment manifests.

## How to tell it is working

- `git remote -v` identifies the repository as `github.com:aliwatters/aliwatters.git`.
- `README.md` remains a tracked file at the repository root.
- The profile-repository marker in `README.md` continues to name `aliwatters/aliwatters`.
- `git ls-files` lists only `README.md` and `CLAUDE.md`, preserving the repository's documentation-only scope.

## Where it fits

GitHub consumes the top-level `README.md` as the `aliwatters` profile page content, as documented in `CLAUDE.md`. The repository has no evidenced runtime dependency, deployment target, or downstream software consumer.
