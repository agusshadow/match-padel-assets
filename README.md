# match-padel-assets

Public image host for screenshots embedded in `match-padel-web` and `match-padel-api` PR descriptions.

Public on purpose: `raw.githubusercontent.com` only works without authentication for public repos. Neither `match-padel-web` nor `match-padel-api` is public, so their own PR bodies can't embed images from their own history — this repo exists only to host those images.

## Contents
Nothing sensitive lives here — only UI screenshots taken for PR review. Never commit secrets, tokens, or any file that isn't a screenshot.

## Layout
`<source-repo>/pr-<number>/<app>-<screen-slug>-{before|after}.png`

Example: `match-padel-web/pr-15/app-auth-after.png`

## Usage
Referenced from a PR body as:
```
![<app> <screen-slug> <before|after>](https://raw.githubusercontent.com/agusshadow/match-padel-assets/main/<source-repo>/pr-<number>/<file>.png)
```
