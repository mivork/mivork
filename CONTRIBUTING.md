# Contributing

*Languages: [English](CONTRIBUTING.md) · [日本語](CONTRIBUTING.ja.md) · [한국어](CONTRIBUTING.ko.md)*

This repository is the profile of mivork. Collaborators are welcome.

## Collaborators

- Collaborators are invited from **Settings → Collaborators** on GitHub.
- Invited collaborators can propose changes through Issues, PRs, and commits.

## Commit rules

- Write commit messages in [Conventional Commits](https://www.conventionalcommits.org/) format (for example `docs:`, `ci:`, `chore:`).
- For commits written with AI assistance, add this co-author line:

  ```text
  Co-Authored-By: Claude Haiku 5.5 <noreply@anthropic.com>
  ```

- Do not push directly to `main`. Create a branch and open a PR.

## Issues and PRs

- When you open an Issue or PR, an automatic first reply is posted based on its type and language. The maintainer will follow up later.
- If a reply seems inaccurate, feel free to comment.

## Automation

| Workflow | Description |
| --- | --- |
| `ai-first-reply.yml` | Posts a template first reply when an Issue or PR is opened (no API, free) |
| `daily-commit.yml` | Records activity 5 times a day (09:00, 14:00, 19:00, 00:00, 05:00 JST) |

Set the following repository secret:

- `GIT_AUTHOR_EMAIL`: the author email for automatic commits (must be linked to your GitHub account)

The first reply detects the item type and language and returns a template, so no API key is needed.
