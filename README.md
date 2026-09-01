# dankaufmann.github.io

Source for the personal academic website of Daniel Kaufmann,
migrated from dankaufmann.com (previously hosted on Wix).

Built with Jekyll; GitHub Pages builds it natively on push to `main`.

## Layout

| Path | Purpose |
| --- | --- |
| `_config.yml` | Site settings, navigation, draft-phase `noindex` flag |
| `_layouts/` | Page templates |
| `assets/css/` | Stylesheet |
| `assets/img/` | Images (portrait, charts) |
| `files/` | Downloadables — `cv.pdf` (linked directly from the nav), dataset CSVs |
| `_archive/` | Retired pages, excluded from the build |
| `*.md` | Page content — `index.md` (bio, news, contact), `research.md`, `data.md` |

## Draft phase

`noindex: true` in `_config.yml` emits a `noindex, nofollow` meta tag on every
page, and `robots.txt` disallows all crawlers. Both must be reverted at launch.

## Editing

Pages are plain Markdown and can be edited directly in the GitHub web UI;
the site rebuilds automatically on commit.
