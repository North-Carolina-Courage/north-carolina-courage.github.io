# north-carolina-courage.github.io

The organization site for the North-Carolina-Courage GitHub organization. Its only job is the custom domain **team.nccourage.com**: because this site uses that domain, every other repository in the organization that publishes a GitHub Pages site is served at `team.nccourage.com/<repository name>` (for example team.nccourage.com/rbediner, and team.nccourage.com/all for The Squad). partners.nccourage.com keeps its own domain.

- `index.html` sends visitors from team.nccourage.com to The Squad (/all/).
- DNS (GoDaddy): CNAME `team` -> `north-carolina-courage.github.io`, plus the GitHub Pages verification TXT record `_github-pages-challenge-North-Carolina-Courage`. Both must stay.
- Do not delete or rename this repository: every staff page moves back to north-carolina-courage.github.io/<name> if it goes.

## Change log

- 2026-10-09: Created with custom domain team.nccourage.com.
