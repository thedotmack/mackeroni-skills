# Claude Code Plugin Release Skill /version-bump

A specialized skill for managing semantic versioning, build distribution, and automated release workflows for Claude Code plugins.

## Features

- **Semantic Versioning**: Automated alignment of `package.json`, `marketplace.json`, and `plugin.json`.
- **Build & Distribution**: Ensures all build artifacts are generated and included in the release commit.
- **Git Integration**: Automated tagging (`vX.Y.Z`) and main branch synchronization.
- **GitHub Release**: Creates rich GitHub releases with detailed notes.
- **Automated Changelog**: Regenerates `CHANGELOG.md` directly from the repository's GitHub releases.
- **Messaging Integration**: Sends release notifications to Discord via webhooks.

## Installation

To use this skill with Claude Code:

1. Clone or copy this repository to your `.claude/skills` directory:
   ```bash
   cp -r ~/Scripts/version-bump ~/.claude/skills/
   ```

## Usage

Once installed, trigger the skill in Claude Code:

> "Use the version-bump skill to patch"
> "Bump version to 11.0.0 using the version-bump skill"

## Workflow Summary

1. **Alignment**: Verifies version strings across all config files.
2. **Build**: Runs `npm run build` to generate fresh artifacts.
3. **Commit**: Stages ALL changes including artifacts.
4. **Tag**: Creates an annotated git tag.
5. **Release**: Publishes a GitHub release with notes.
6. **Changelog**: Updates the project's changelog from the release history.
7. **Notify**: Triggers a Discord notification.
