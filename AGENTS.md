# AGENTS.md

## Cursor Cloud specific instructions

### Repository nature (important)

This repository (`github/dev`) is **documentation-only**. It is the placeholder/landing
repo for the hosted **github.dev** browser-based VS Code editor — the actual editor
source is **not** in this repo.

The only tracked content is `README.md`. There is intentionally:

- No application/source code to run.
- No `package.json`, lockfiles, or any dependency manifest.
- No build, lint, or test tooling, and no CI configuration.

### Consequences for setup / build / run / test

- There is **nothing to install**. The startup update script is a no-op.
- There is **no service to start** and **no application to run** locally. The github.dev
  product itself is a hosted GitHub service, reached by pressing `.` on a repo or swapping
  `.com` → `.dev` in a GitHub URL (e.g. `https://github.dev/github/dev`); it cannot be run
  from this repository.
- There are **no automated tests, lint, or build commands**.
- The only meaningful "output" of this repo is the rendered `README.md` (as GitHub
  displays it). Verify changes by previewing the Markdown.
