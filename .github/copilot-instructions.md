# GitHub Copilot Instructions

This file provides repository-level context for GitHub Copilot and Copilot-powered
workflows (e.g. Copilot Workspace, Copilot coding agent).

## Repository Purpose

This is the `.github` repository for the [@abuxton](https://github.com/abuxton)
GitHub organisation. It holds the **default community health files** that GitHub
automatically applies to every repository in the organisation that does not
provide its own copy.

Files in this repository define shared standards for:
- Issue and pull-request templates
- Code of conduct, contributing guidelines, security policy, and support docs
- Code ownership (`CODEOWNERS`)

## Writing Style

- Use clear, concise, imperative language.
- Prefer plain Markdown; avoid raw HTML unless strictly necessary.
- Headings should use sentence case (e.g. `## Reporting a vulnerability`).
- Keep line length ≤ 120 characters.

## Issue & PR Templates

- Issue templates live in `.github/ISSUE_TEMPLATE/` as **YAML Issue Forms**
  (`*.yml`).  Do not use the legacy frontmatter-only Markdown format.
- The PR template lives at `.github/PULL_REQUEST_TEMPLATE.md`.
- When updating templates, ensure every template includes:
  - Clear acceptance criteria or reproduction steps.
  - A *Relevant Files or Modules* / *Implementation Notes* field so that
    automated tools have enough context to act on the issue.
  - A pre-submission checklist with `required: true` for mandatory items.

## Commit Message Convention

Follow [Conventional Commits](https://www.conventionalcommits.org/):

```
feat: add support for X
fix: resolve Y when Z
docs: update contributing guide
chore: bump dependency versions
```

## Key Files

| File | Role |
|---|---|
| `CODE_OF_CONDUCT.md` | Contributor Covenant 2.1 |
| `CONTRIBUTING.md` | Contribution guidelines |
| `SECURITY.md` | Vulnerability reporting process |
| `SUPPORT.md` | Getting help |
| `CODEOWNERS` | Default ownership rules |
| `.github/PULL_REQUEST_TEMPLATE.md` | PR template |
| `.github/ISSUE_TEMPLATE/bug_report.yml` | Bug report form |
| `.github/ISSUE_TEMPLATE/feature_request.yml` | Feature request form |
| `.github/ISSUE_TEMPLATE/config.yml` | Issue template chooser config |
