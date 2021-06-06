# Github Actions
Github actions exploration

# Git strategy

## Branches
- `main` - The default branch
- `devops` - For devops feature
- `bugs` - For bug fixes
- `testing` - internal testing
- `alpha` - closed testing
- `beta` - open testing
- `prod` - live

## Strategy
- All development to be done based out of `feature branches`.
- PR to be raised to `feature branches` on completion of development.
- `feature branches` -> `main` - on completion of feature.
- `main` -> `testing` - when testing is required
- `testing` -> `alpha` - when alpha build is required
- `alpha` -> `beta` - when alpha build is required
- `beta` -> `prod` - when alpha build is required

# Devops 

### Push and PR to main and devops

- Build
- Run tests
- Upload **debug** APK files

### Push and PR to testing

- Build
- Run tests
- Upload **debug** APK files
- Deploy to *Firebase app distribution* or *Internal testing track*.

### Push and PR to alpha

- Build
- Run tests
- Upload **signed** APK files
- Deploy to **aplha** track.

### Push and PR to beta

- Build
- Run tests
- Upload **signed** APK files
- Deploy to **beta** track.

### Push and PR to prod

- Build
- Run tests
- Upload **signed** APK files
- Deploy to **production** track.
