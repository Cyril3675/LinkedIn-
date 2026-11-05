# Vendored: linkedin-skills

Copied from https://github.com/sergebulaev/linkedin-skills (MIT, see `LICENSE`)
at commit `8f8bc4b40a2d5419b2dcf898772b85712cfbdf41` (plugin version 1.1.28).

Why vendored: `/plugin` is not available in Claude Code cloud sessions, so the
skills are committed as project skills under `.claude/skills/`.

Layout mirrors the upstream plugin root with `.claude/` as root, so the skills'
relative paths (`../../references/...`, `lib/...`, `scripts/...`) still resolve.

Optional API features (publishing via Publora, scraping via Apify, images via
Pixfaro, AI detectors) need keys: copy `.claude/.env.example` to `.claude/.env`
(git-ignored). Python deps: `pip install -r .claude/requirements.txt`.

To update: re-clone upstream and copy `skills/`, `references/`, `lib/`,
`scripts/`, `requirements*.txt`, `SKILL.md` over these files.
