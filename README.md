# Submodule-update
A GitHub action that automatically creates PR to update submodules to their latest version.

## Example
```
name: "Open pull request for submodule updates"
on:
  schedule:
    - cron: "30 1 * * *"

jobs:
  stale:
    runs-on: ubuntu-latest
    steps:
      - uses: mathdugre/submodule-update@v0.2
        with:
          token: ${{ secrets.GITHUB_TOKEN }}
```
