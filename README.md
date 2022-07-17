# GG [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](LICENSE.md)

GG speeds up the creation of those pesky single commit merge requests by combiding several steps into one.

Written example:

```bash
➜ gg feature/typo-in-readme "Fix a typo in the README.md"
```

## Contents

1. [Requirements](#requirements)
2. [Installations](#installation)
3. [Updating](#updating)
4. [Uninstall](#uninstall)
5. [How it works](#how-it-works)
6. [Settings](#settings)
7. [License](#license-gnu-general-public-license-v3)

## Requirements

- Git

##### [Back to Contents](#contents)

## Installation

On macOS or Linux, you can install *GG* via [Homebrew](https://brew.sh/):

```bash
brew tap nicasso/gg
brew install gg
```

Changes are only available in a new shell session. To make changes immediately
available, run `source ~/.bashrc` (or your shell config file like `.zshrc`).

##### [Back to Contents](#contents)

## Updating

```bash
brew update gg --upgrade
```

## Uninstall

To remove *GG*:

```bash
brew uninstall gg
brew untap nicaso/gg
```

## How it works

*GG* handles multiple git commands for you for faster and easier single commit merge requests.

* `checkout` &ndash; adds `-Q` to `ag` when suggested;
* `commit` &ndash; fixes misspelled commands like `aws dynamdb scan`;
* `push` &ndash; fixes misspelled commands like `az providers`;
* `open merge request url` &ndash; fixes misspelled commands like `az providers`;
* `checkout to previous repo` &ndash; fixes misspelled commands like `az providers`;

##### [Back to Contents](#contents)

## Settings

*GG* has no settings yet, but get have them in the future for more customization.

##### [Back to Contents](#contents)

## License GNU General Public License V3
Project License can be found [here](LICENSE.md).

##### [Back to Contents](#contents)