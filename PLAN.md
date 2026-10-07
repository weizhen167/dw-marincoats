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
4. [x] Commit, push, and verify the GitHub Pages deployment.

## Progress

- Confirmed the replacement is a buildless bilingual static site with 24 HTML pages.
- Confirmed all local HTML and CSS references resolve to existing files.
- Confirmed `app.js` passes Node syntax validation.
- Promoted the replacement content to the repository root and removed the old site from the current tree.

## Current milestone

- Complete.

## Decisions

- Preserve `CNAME`, Git metadata, and the deployment branch.
- Keep the supplied `DW-Marincoats-Website` folder locally as an ignored source copy.
- Retain the old version in Git history rather than as duplicate live files.

## Validation

- Local references: 0 missing.
- JavaScript syntax: passed.
- GitHub Pages build: passed.
- HTTPS and custom-domain enforcement: enabled.
- Production pages, stylesheet, script, image, video, and PDF checks: HTTP 200.

## Blockers

- None.

## About-page copy update — 2026-10-07

- Scope: replace the highlighted introduction with the supplied Chinese and English wording; preserve headings and layout.
- Progress: updated both live-source pages, their description metadata, and the ignored local source copies; published the update through the existing GitHub Pages integration.
- Current milestone: complete.
- Decisions: keep the screenshot wording verbatim and synchronize visible copy with page/share descriptions.
- Validation: exact-copy replacement and source-copy synchronization passed; local HTML references have 0 missing targets; JavaScript syntax and diff whitespace checks passed. GitHub Pages built commit 5053214 successfully; both public about pages returned HTTP 200 with the new copy in all 3 locations and the old copy absent. This buildless static site has no package test/lint/build scripts.
- Blockers: none.

## Homepage production-base image update — 2026-10-07

- Scope: replace the homepage introduction's main factory photo with the supplied Shandong Dowill photo in both languages; preserve the laboratory inset and other uses of the existing factory photo.
- Progress: added the supplied original PNG, updated both homepage references and ignored source copies, and published the replacement.
- Current milestone: complete.
- Decisions: retain the existing image layout and use a dedicated asset to avoid changing unrelated sections.
- Validation: both pages differ only in the requested image reference and alt text; source copies match; both asset copies match the supplied file by SHA-256; local HTML links, JavaScript syntax, and diff whitespace checks passed. GitHub Pages built commit 4b9fdc6 successfully; both public homepages return HTTP 200 with the replacement reference, and the live PNG matches the original by SHA-256. Browser visual check confirms the new photo and preserved laboratory inset at the desktop breakpoint.
- Blockers: none.
