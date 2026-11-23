# north-carolina-courage.github.io

The organization site for the North-Carolina-Courage GitHub organization. Its only job is the custom domain **team.nccourage.com**: because this site uses that domain, every other repository in the organization that publishes a GitHub Pages site is served at `team.nccourage.com/<repository name>` (for example team.nccourage.com/rbediner, and team.nccourage.com/all for The Squad). partners.nccourage.com keeps its own domain.

- `index.html` sends visitors from team.nccourage.com to The Squad (/all/).
- DNS (GoDaddy): CNAME `team` -> `north-carolina-courage.github.io`, plus the GitHub Pages verification TXT record `_github-pages-challenge-North-Carolina-Courage`. Both must stay.
- Do not delete or rename this repository: every staff page moves back to north-carolina-courage.github.io/<name> if it goes.

## Starting something new

Every new hub, page or app for staff is its own repo, created from the Club template:
`gh repo create North-Carolina-Courage/<name> --private --template North-Carolina-Courage/club-app-template`.
The repo's name is its address, `team.nccourage.com/<name>`. The template's README has the steps.

### Naming

- A department's hub takes the department's name: `marketing`, `operations`, `finance`, `hr`, `technology`. Business
  Operations' hub is The Den, at `den`.
- A product takes `<department>-<product>` (for example `finance-budget`), or a short name of its own if it serves the
  whole Club (for example `store`).

### The app list

`apps.json` lists every hub, page and app, one entry per repo: `name`, `repo`, `address`, `department`
(`business-operations`, `marketing`, `operations`, `finance`, `hr`, `technology` or `club`), `kind` (`hub`, `page` or `app`)
and `sign_in` (`true` when it opens behind the Club sign-in). Add a product's entry through a pull request when it goes
live. The file is public: no names of people, nothing private.

## Change log

- 2026-10-09: Created with custom domain team.nccourage.com.
- 2026-11-22: Added `apps.json` (the Club's app list) and the naming rule; new repos start from `club-app-template`.
