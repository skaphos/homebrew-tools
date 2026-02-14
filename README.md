# homebrew-tools

Homebrew tap repository for Skaphos tooling formulae.

## Bootstrap

1. Add a formula file to `Formula/`, for example `Formula/skaphos-tool.rb`.
2. Open a pull request; `Tap CI` validates style, audit, and source builds.
3. Merge to `main` to keep the tap publishable.

## Use the tap

```bash
brew tap skaphos/tools https://github.com/skaphos/homebrew-tools
brew install skaphos/tools/<formula-name>
```

## Local validation

```bash
brew style Formula/*.rb
brew audit --strict --online Formula/*.rb
brew install --build-from-source Formula/<formula-name>.rb
```
