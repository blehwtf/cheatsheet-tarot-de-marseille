# Tarot de Marseille — Reader's Cheat Sheet

A single-page static reference for all 78 cards of the Tarot de Marseille: Major Arcana imagery, pip card meanings, court card meanings, suit domains, and pochoir color symbolism.

Built with [nanoc](https://nanoc.app).

## Development

**Prerequisites:** Ruby 3.3+ via [rbenv](https://github.com/rbenv/rbenv) or [asdf](https://asdf-vm.com).

```sh
bundle install
bundle exec nanoc compile
bundle exec nanoc view        # http://localhost:3000
```

### Checks

```sh
bundle exec nanoc check fs    # internal link integrity
bundle exec nanoc check css   # CSS validity
bundle exec rubocop           # Ruby style
```

### Pre-commit hooks

```sh
brew install pre-commit
pre-commit install
```

## Build output

`nanoc compile` writes to `output/` (git-ignored). Deploy the contents of that directory to any static host.
