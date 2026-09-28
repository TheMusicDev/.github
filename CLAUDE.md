# CLAUDE.md

Profile README for TheMusicDev LLC (org-level GitHub profile). Single rendered file:
`profile/README.md` (+ `profile/assets/hero.svg`). Live at https://github.com/TheMusicDev.

## Ground rules

- Working-tree edits only. Never stage/commit/push unless explicitly asked (user global rule).
- Public-facing copy: keep the music-industry voice (setlist/encore metaphors) used in the README.
- README links must point at real repos; verify with the org listing
  (https://github.com/orgs/TheMusicDev/repositories) before adding one.
- Packages referenced in the README (composer/bun) should be live on Packagist or npm
  before quoting the install command.

## Public repos inventory (verified 2026-09-28)

- cakephp-daisyui + cakephp-daisyui-docs — daisyUI 5 view helpers for CakePHP 5; plugin on Packagist (`themusicdev/cakephp-daisyui` v1.0.0)
- env-sync — monorepo .env sync, Bun/TS, npm `@themusicdev/env-sync`
- jamendo-ts-client + jamendo-openapi — Jamendo API client + OpenAPI spec
- ollert-monorepo — stripped-down Trello clone (CakePHP, TanStack Start, Supabase)

## Learnings log (append; newest first)

- 2026-09-28: cakephp-daisyui review — codebase mature: 76 test files, phpstan 2, phpcs,
  CI, conventional commits, strict types, output escaped via `h()`, CDN assets SRI-pinned.
  Open improvement ideas: (1) modal uses inline `onclick="showModal()"` — CSP-unsafe,
  README acknowledges it; a data-attribute/`<dialog>`-based progressive-enhancement path
  would remove the `unsafe-inline` need; (2) CDN pins (daisyui@5.7.46, tailwind 4.3.3)
  need a bump ritual per upstream release; (3) profile README's "setlist" stack lists
  TypeScript only while org ships major PHP/CakePHP work — consider a PHP line.