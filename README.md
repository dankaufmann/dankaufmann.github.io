# dankaufmann.github.io

Source for the personal academic website of Daniel Kaufmann,
migrated from dankaufmann.com.

Built with Jekyll; GitHub Pages builds it natively on push to `main`.

## Layout

| Path | Purpose |
| --- | --- |
| `_config.yml` | Site settings, navigation, draft-phase `noindex` flag |
| `_layouts/` | Page templates |
| `assets/css/` | Stylesheet |
| `assets/img/` | Images (portrait, charts) |
| `files/` | Downloadables — `CV_DanielKaufmann.pdf` (linked directly from the nav), dataset CSVs |
| `_archive/` | Retired pages, excluded from the build |
| `*.md` | Page content — `index.md` (bio, news, contact), `research.md`, `data.md` |

## Draft phase

A single flag, `noindex: true` in `_config.yml`, controls three things:

1. a `noindex, nofollow` meta tag on every page,
2. `robots.txt` disallowing all crawlers,
3. the work-in-progress banner pointing visitors at dankaufmann.com.

Setting it to `false` at launch removes all three at once. Nothing else needs
to be remembered.

## Editing

Pages are plain Markdown and can be edited directly in the GitHub web UI;
the site rebuilds automatically on commit.
