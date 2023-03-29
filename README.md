# npm Packages Install Action

[![Release version badge](https://img.shields.io/github/v/release/chvmvd/npm-packages-install-action.svg?logo=github)](https://github.com/chvmvd/npm-packages-install-action/releases)
[![license](https://img.shields.io/badge/license-MIT-informational.svg)](LICENSE)
![PRs](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)

This action installs npm packages.

## Table of Contents

- [npm Packages Install Action](#npm-packages-install-action)
  - [Table of Contents](#table-of-contents)
  - [About](#about)
  - [Usage](#usage)
  - [Configuration](#configuration)
    - [Inputs](#inputs)
    - [Outputs](#outputs)
  - [License](#license)
  - [Contributing](#contributing)

## About

This action installs npm packages.

## Usage

You can use this action in your workflow by writing like this:

```yaml
name: Install npm Packages

on:
  pull_request:

jobs:
  install:
    name: Install npm Packages
    runs-on: ubuntu-latest
    steps:
      - name: Checkout
        uses: actions/checkout@v3

      - name: Install npm Packages
        uses: chvmvd/npm-packages-install-action@v1.0.0
        with:
          path: "."
```

## Configuration

### Inputs

| Name   | Description                                                     | Default |
| ------ | --------------------------------------------------------------- | ------- |
| `path` | The path to the directory where package-lock.json is located in | `.`     |

### Outputs

None.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Contributing

Issues and pull requests are always welcome.
