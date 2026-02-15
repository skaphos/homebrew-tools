# homebrew-tools

Homebrew tap repository for Skaphos tooling formulae and casks.

## Bootstrap

1. Add a formula file to `Formula/` (for CLI/tools) or a cask file to `Casks/` (for app bundles).
2. Open a pull request; `Tap CI` validates style, audit, and source builds.
3. Merge to `main` to keep the tap publishable.

## Use the tap

```bash
brew tap skaphos/tools https://github.com/skaphos/homebrew-tools
brew install skaphos/tools/<formula-name>
brew install --cask skaphos/tools/<cask-token>
```

## Local validation

```bash
brew style Formula/*.rb
brew audit --strict --online Formula/*.rb
brew install --build-from-source Formula/<formula-name>.rb

brew style Casks/*.rb
brew audit --cask --strict --online Casks/*.rb
```
