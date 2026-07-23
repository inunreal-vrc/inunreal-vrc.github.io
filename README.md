# inunreal-vrc.github.io static assets CDN

This repository is configured to act as a static asset host.

## Asset folder

Place all static assets under `/assets`.

Example path in repository:

- `/assets/images/banner.png`

Public URL pattern:

- `https://raw.githubusercontent.com/inunreal-vrc/inunreal-vrc.github.io/main/assets/images/banner.png`

## Git LFS setup

This repository tracks common static asset extensions with Git LFS via `.gitattributes`.

If you have not enabled LFS locally:

```bash
git lfs install
git lfs pull
```

## CI check

A GitHub Actions workflow validates that:

1. Static asset files are placed under `/assets`
2. Matching static asset files are tracked by Git LFS
