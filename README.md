# GG [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](LICENSE.md)

*GG* speeds up the creation of those pesky single commit merge requests by combining several (Git) commands into one.

Written example:

```bash
➜ gg feature/typo-in-readme "Fix a typo in the README.md"
```

# Notice

It currently only works for Github, Gitlab, and Bitbucket merge requests (or pull requests depending on the platform).

## Contents

1. [Requirements](#requirements)
2. [Installations](#installation)
3. [Updating](#updating)
4. [Uninstall](#uninstall)
5. [How it works](#how-it-works)
6. [To-do](#to-do)
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

##### [Back to Contents](#contents)

## Updating

```bash
brew update gg --upgrade
```

## Uninstall

To remove *GG*:

##### [Back to Contents](#contents)

```bash
brew uninstall gg
brew untap nicaso/gg
```

##### [Back to Contents](#contents)

## How it works

*GG* combines multiple (Git) commands for you, for faster and easier single commit merge requests.

1. `git checkout` First it creates a new branch with the provided name;
2. `git commit` Then it creates the commit with the provided commit message;
3. `git push` After that it pushes to the created branch;
4. `open` Then it looks for the url used for creating a new merge request in the response of the git push command and opens that page in your browser;
5. `git checkout` Finally it does a checkout back to the repository you started from;

##### [Back to Contents](#contents)

## To-do

There are still some things that could be created in the future.

- Supporting multiline commit messages.

##### [Back to Contents](#contents)

## License GNU General Public License V3
Project License can be found [here](LICENSE.md).

##### [Back to Contents](#contents)