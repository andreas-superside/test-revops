# Team to Enterprise Release

## What it is

A RevOps proposal page for moving artifacts from a department Team workspace to the Enterprise workspace, with GitHub as the source. It covers:

- Part 1, artifact sharing: the four-step process, how to update after release, what every team needs, the pilot results and what is still to test.
- Part 2, skill sharing: in the works, with open questions.

Version 1.2.0 replaces the earlier throwaway "Release Test" page in this folder. The Team and Enterprise links stay the same.

## How it was built

1. Provided by the owner as a finished single HTML file (`artifact.html`) and committed unchanged on 2026-11-09.
2. Styles are inline. The only external resource is Inter Tight and Raleway from Google Fonts, with system fallbacks. No scripts, no data, no runtime capabilities.
3. Supports light and dark themes through CSS color tokens. Works at phone width.
4. `artifact.html` in this folder is the clean release version. It never contains the "Dev copy" banner.

## Files

| File | Purpose |
|---|---|
| `artifact.html` | The clean page source that Enterprise publishes |
| `spec.md` | This description |
| `release.json` | Release metadata: name, version, Team link, Enterprise link, status |

## Banner rule

The Team copy (`team_link`) is published with a "Dev copy. Use this link instead: [enterprise_link]" banner added at publish time only. The banner is never committed here, so an Enterprise refresh always publishes a clean page.

## How to release

In the Enterprise session, republish `release-test/artifact.html` from this repo unchanged to the existing `enterprise_link`, keeping the same link, and set `status` to `published`.
