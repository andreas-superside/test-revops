# Release Test

## What it is

A throwaway one-page artifact used to test the release flow from the Team workspace to the Enterprise workspace through GitHub. It shows:

- Title: Release Test
- Version: 1.0.0
- Date: 2026-11-09

It has no data, no scripts and no runtime capabilities.

## How it was built

1. Written by hand as a single HTML file (`artifact.html`) in a Claude Code cloud session on 2026-11-09.
2. Styles are inline. The only external resource is IBM Plex Sans and IBM Plex Mono from Google Fonts, with system fallbacks.
3. Supports light and dark themes through CSS color tokens. Works at phone width.
4. Published as a private Claude artifact (Team): https://claude.ai/artifact/S6dWqJP3MVQ6kKyBV2YpYm
5. `artifact.html` in this folder is byte-for-byte the file that was published.

## Files

| File | Purpose |
|---|---|
| `artifact.html` | The exact published page source |
| `spec.md` | This description |
| `release.json` | Release metadata: name, version, Team link, Enterprise link (empty until released), status |

## How to release

In the Enterprise session, publish `release-test/artifact.html` from this repo unchanged as a new artifact, then set `enterprise_link` in `release.json` to the new URL and `status` to `released`.
