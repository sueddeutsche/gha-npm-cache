# Github Action NPM cache

Caches npm between builds.

## Usage

Use it in a workflow like this:

```yaml
name: My workflow
on:
  push:

jobs:
  test:
    name: Test
    runs-on: ubuntu-latest
    steps:
      - uses: actions/checkout@v2
      - uses: sueddeutsche/gha-npm-cache
      - run: npm i
```