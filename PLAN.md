# Deployment plan

## Scope and acceptance criteria

- Replace the currently published website with the rewritten static site.
- Preserve the existing `www.dwmarincoats.com` custom-domain configuration.
- Publish from `main` through the existing GitHub Pages integration.
- Verify local assets, JavaScript, deployment completion, and the public site.

## Milestones

1. [x] Inspect the replacement site and repository state.
2. [x] Validate local links, assets, and JavaScript syntax.
3. [x] Replace the old site tree while preserving Git history and domain configuration.
4. [ ] Commit, push, and verify the GitHub Pages deployment.

## Progress

- Confirmed the replacement is a buildless bilingual static site with 24 HTML pages.
- Confirmed all local HTML and CSS references resolve to existing files.
- Confirmed `app.js` passes Node syntax validation.
- Promoted the replacement content to the repository root and removed the old site from the current tree.

## Current milestone

- Commit, publish, and validate the production deployment.

## Decisions

- Preserve `CNAME`, Git metadata, and the deployment branch.
- Keep the supplied `DW-Marincoats-Website` folder locally as an ignored source copy.
- Retain the old version in Git history rather than as duplicate live files.

## Validation

- Local references: 0 missing.
- JavaScript syntax: passed.
- Production deployment: pending.

## Blockers

- None.
