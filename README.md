# GG [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](LICENSE.md)

*GG* speeds up the creation of those pesky single commit merge requests by combining several (Git) commands into one.

It currently supports Github, Gitlab, and Bitbucket merge requests (or pull requests depending on the platform).

Written example including the commit message:

```bash
➜ gg feature/typo-in-readme "Fix a typo in the README.md"
```

Written example where you can add the commit message in your favourite text editor:

```bash
➜ gg feature/typo-in-readme
```

Demo:

![Demo](assets/demo.gif)

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
brew update && brew upgrade nicasso/gg/gg
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

Nothing I can think of for now. If you have any suggestions, please open an issue.

##### [Back to Contents](#contents)

## License GNU General Public License V3
Project License can be found [here](LICENSE.md).

##### [Back to Contents](#contents)
