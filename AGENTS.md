# AGENTS.md

## Cursor Cloud specific instructions

### What this repository is

This repository is a **documentation-only** boundary for DUBSAR. It contains
Markdown docs (root `*.md`, `docs/`, `rfcs/`, `examples/`) plus brand assets
(`brand/*.svg`, `brand/*.png`) and one historical `LICENSE.txt`. See
[`README.md`](README.md) and [`INSTALLATION.md`](INSTALLATION.md) for the
authoritative statement of scope.

There is intentionally **no application code, no package manifest, no build
system, no automated test suite, no linter config, and no CI** in this tree.
Do not fabricate one or reconstruct the retired plugin/marketplace trees
(explicitly forbidden by `INSTALLATION.md`). The "product" here is the rendered
documentation content itself.

### Environment / dependencies

Nothing needs to be installed to work on this repo — the startup update script
is a no-op. The VM already provides Node.js, `npx`, Python 3, and `git`, which
is all that the optional preview/validation workflows below need.

### Developer workflows (all optional, none required to commit)

These are the closest equivalents to "build / test / run" for a docs repo.
None are configured in-repo; run them ad hoc. Work outside the repo tree
(e.g. `/tmp`) so you never commit generated HTML or `node_modules`.

- Preview / "build+run": render Markdown to HTML and serve it. A quick way with
  no repo changes:
  - `npx marked <file>.md > /tmp/out.html` to render a single file
    (needs network to the npm registry the first time), or
  - `python3 -m http.server` to serve files locally.
- "Test": validate that internal links and image references resolve. There is
  no bundled checker; a small script that walks the `*.md` files and checks each
  relative link/image target against the filesystem is sufficient (external
  `http(s)`/`mailto` links are not fetched). As of this writing all 93 internal
  references across the 36 Markdown files resolve.

### Gotchas

- `python3 -m venv` fails in this VM (`ensurepip` / `python3-venv` not
  installed). Prefer Node/`npx` tooling, or `pip install --user`, instead of
  virtualenvs for throwaway doc tooling.
- Keep any rendered output and installed tooling out of the repo — there is no
  `.gitignore` policy for build artifacts because the repo has no build.
