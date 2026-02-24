---
name: release-and-auto-changelog
description: Generic automated semantic versioning and release workflow. Handles version increments, git tagging, GitHub releases, and automated changelog generation for any repository.
---

# Release & Auto-Changelog Workflow

**IMPORTANT:** You must first plan and write detailed release notes before starting the version bump workflow.

**CRITICAL:** ALWAYS commit EVERYTHING (including build artifacts). At the end of this workflow, NOTHING should be left uncommitted or unpushed. Run `git status` at the end to verify.

## Preparation

1.  **Analyze**: Determine if the change is a **PATCH** (bug fixes), **MINOR** (features), or **MAJOR** (breaking) update.
2.  **Environment**: Identify the repository owner and name (e.g., from `git remote -v`).
3.  **Files**: Identify which files contain version strings (e.g., `package.json`, `VERSION`, `pyproject.toml`).

## Workflow

1.  **Update**: Increment version strings in relevant configuration files.
2.  **Verify**: Ensure all files match the new version.
3.  **Build**: Run any necessary build or distribution scripts.
4.  **Commit**: Stage all changes: `git add -A && git commit -m "chore: bump version to X.Y.Z"`.
5.  **Tag**: Create an annotated tag: `git tag -a vX.Y.Z -m "Version X.Y.Z"`.
6.  **Push**: `git push origin main && git push origin vX.Y.Z`.
7.  **Release**: `gh release create vX.Y.Z --title "vX.Y.Z" --notes "RELEASE_NOTES"`.
8.  **Changelog**: Regenerate `CHANGELOG.md` using the GitHub API and the provided script:
    ```bash
    gh api repos/{owner}/{repo}/releases --paginate | ./scripts/generate_changelog.js > CHANGELOG.md
    ```
9.  **Sync**: Commit and push the updated `CHANGELOG.md`.
10. **Finalize**: Run `git status` to ensure a clean working tree.

## Checklist

- [ ] All version files updated and verified
- [ ] Build/Distribution successful
- [ ] Git tag created and pushed
- [ ] GitHub release created with notes
- [ ] `CHANGELOG.md` updated and pushed
- [ ] `git status` shows clean tree
