# Contributing

## Setup

```sh
git clone https://github.com/blehwtf/tarotreading.git
cd tarotreading
bundle install
pre-commit install
```

Requires Ruby 3.3+ ([rbenv](https://github.com/rbenv/rbenv) or [asdf](https://asdf-vm.com)) and [pre-commit](https://pre-commit.com).

## Workflow

```sh
bundle exec nanoc compile     # build site to output/
bundle exec nanoc view        # dev server at http://localhost:3000
```

## Before opening a PR

Pre-commit runs automatically on `git commit`. To run all checks manually:

```sh
pre-commit run --all-files
```

Individual checks:

```sh
bundle exec rubocop           # Ruby style
bundle exec nanoc check fs    # internal link integrity
bundle exec nanoc check css   # CSS validity
```

## What to contribute

- Corrections to card descriptions or meanings
- Accuracy improvements to French/English names and numbering
- Layout, accessibility, or CSS fixes
- nanoc tooling improvements

## What not to change

The card interpretations reflect a specific, internally consistent framework (the plant-cycle pip system and astrological court correspondences). Changes to meaning content should be clearly sourced.
