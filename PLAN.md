# Deployment plan

## Scope and acceptance criteria

- Publish the existing static website on a free hosted URL.
- Keep `style-a/index.html` and all `shared` images, downloads, and video working.
- Connect deployment to Git so every push to `main` republishes automatically.

## Milestones

1. [x] Inspect the site structure, assets, Git state, and available account access.
2. [x] Add a root entry page suitable for branch-based GitHub Pages hosting.
3. [x] Create and push the GitHub repository, then enable Pages.
4. [x] Verify the deployment and its public URL.

## Progress

- Confirmed this is a buildless static site.
- Confirmed all referenced assets live under `shared/` and the largest file is below GitHub's per-file limit.
- Selected branch-based GitHub Pages for free hosting and automatic publishing on every push to `main`.

## Current milestone

- Complete.

## Decisions

- Preserve the supplied source tree and use a small root page that redirects to `style-a/`.
- Publish directly from the `main` branch so no custom workflow permission is required.

## Validation

- Source resource references inspected.
- GitHub Pages build completed successfully.
- Public root page, website page, hero image, MP4 video, and an encoded PDF download all returned HTTP 200.

## Blockers

- None.
