# Git-Plugin

`git-plugin` is a command-line tool for managing your Vim plugins using Git
submodules. It simplifies the process of adding, moving, and removing Vim
plugins, allowing you to manage them with ease.

While you can probably use this for general submodule management, it has been
specifically developed for this purpose. YMMV.

## Features

- Add Vim plugins as Git submodules
- Move Vim plugins between pack directories
- Remove Vim plugins by deleting the corresponding Git submodules
- List currently installed plugins

## Installation

You can install this using pip:

`pip install https://github.com/harleypig/git-plugin-manager.git`

### Commands

* Add a plugin: `git plugin add https://github.com/username/repo.git`
* Move a plugin: `git plugin move plugin-name pack-directory`
* Remove a plugin: `git plugin remove plugin-name`
* List installed plugins: `git plugin list`

The `plugin-name` is derived from the repository name with `.vim` and `.nvim`
stripped.

## Development

To develop `git-plugin`, you need to clone this repository and install the
required dependencies using [Poetry](https://python-poetry.org/).

These instructions assume you already have poetry installed.

* Clone the repository: `git clone https://github.com/harleypig/git-plugin-manager.git`
* Change to the directory: `cd git-plugin-manager`
* Install the dependencies: `poetry install`
* Build the project: `poetry build`

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for more information.

