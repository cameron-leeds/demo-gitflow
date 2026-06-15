# demo-gitflow
Just trying to demo how gitflow works (albeit antiquated)

## Gitflow Branch Naming Guide

This repository demonstrates a simplified Gitflow-style process with these primary branches:

- `main` — production-ready releases
- `develop` — integration branch for ongoing development

### Feature branches

In this demo, feature branches use a custom prefix instead of the traditional `feature/` prefix:

- `cl/login` — ongoing work for login functionality
- `cl/dashboard` — ongoing dashboard improvements

### Release branch

- `release/1.0.0` — prepare code for a release, test, and final polishing before merging back into `main` and `develop`

### Hotfix branch

- `hotfix/urgent-fix` — fix a critical issue on `main` and merge the fix back into `develop`

### How the workflow works

1. Create feature branches off `develop`.
2. Merge completed feature branches into `develop`.
3. Create release branches from `develop` when you’re ready to stabilize for production.
4. Merge release branches into `main` and back into `develop`.
5. Create hotfix branches from `main` for urgent production fixes, then merge back into both `main` and `develop`.
