# GG [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](LICENSE.md)

*GG* speeds up the creation of those pesky single commit merge requests by combiding several steps into one.

Written example:

```bash
➜ gg feature/typo-in-readme "Fix a typo in the README.md"
```

# Notice

It currently only works for Gitlab merge requests, an update will follow soon for GitHub support.

## Contents

1. [Requirements](#requirements)
2. [Installations](#installation)
3. [Updating](#updating)
4. [Uninstall](#uninstall)
5. [How it works](#how-it-works)
6. [Settings](#settings)
7. [To-do](#to-do)
8. [License](#license-gnu-general-public-license-v3)

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

1. `checkout` First we create a new branch with the provided name;
2. `commit` Then we create the commit with the provided commit message;
3. `push` After that we push to the current branch;
4. `open pull request url` Then we look for the url that creates a pull request and open that in your browser;
5. `checkout to previous repo` Finally we checkout the repo you started from;

##### [Back to Contents](#contents)

## Settings

*GG* has no settings yet, but will probably have them in the future for more customization.

##### [Back to Contents](#contents)

## To-do

There are still some things I need/want to create for this alias.

- Github support with their pull-request URL;
- Bitbucket support with their pull-request URL;
- A couple of customizable features;

##### [Back to Contents](#contents)

## License GNU General Public License V3
Project License can be found [here](LICENSE.md).

##### [Back to Contents](#contents)