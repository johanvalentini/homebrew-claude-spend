# homebrew-claude-spend

Homebrew tap for [claude-spend](https://github.com/johanvalentini/claude-spend), live token
and cost tracking for Claude Code. Works on macOS and Linux.

```sh
brew tap johanvalentini/claude-spend
brew trust johanvalentini/claude-spend
brew install claude-spend
brew services start claude-spend
claude-spend setup
```

The formula is maintained in the main repo under `Formula/claude-spend.rb`. Each release
opens a pull request here; `brew test-bot` (`.github/workflows/tests.yml`) builds bottles
for macOS and Linux, and the `brew pr-pull` workflow (`publish.yml`, dispatched by the
release script) merges the PR with the `bottle` block and uploads the bottles to this
repo's GitHub Releases. `brew install --HEAD claude-spend` builds the main branch instead.
