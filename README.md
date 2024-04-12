

<h1 align="center">Note</h1>

<p align="center">
  <a href="https://github.com/TheK4n">
    <img src="https://img.shields.io/github/followers/TheK4n?label=Follow&style=social">
  </a>
  <a href="https://github.com/TheK4n/note">
    <img src="https://img.shields.io/github/stars/TheK4n/note?style=social">
  </a>
</p>

* [Features](#features)
* [Installation](#installation)
* [Usage](#usage)
* [Roadmap](#roadmap)

---

Simple notes storage mechanism

## Features

* Simple synchronization via git
* FZF Integration
* Friendly zsh and bash completions
* Saving all notes changes with git
* It uses default environment variables such as `EDITOR` and `PAGER`


> [!NOTE]
>
> It is highly recommended to use the `neovim` as editor and `peek.nvim` plugin as markdown previewer


<a id="chapter-1"></a>
## Installation

### Dependencies

Dependencies:
* git

Optional dependencies:
* bat - For render notes in terminal
* tree - Show tree of notes
* fzf - Beauty notes search
* rg - Search notes by content


### Install from source:
```bash
git clone https://github.com/thek4n/note.git
cd note
make install
```

### Install from [AUR](https://aur.archlinux.org/packages/note-manager) (recommended):
```bash
yay -S note-manager
```

### Run tests
```bash
make test
```


## Usage
```bash
export PAGER=less
export EDITOR=nvim
note init -p ~/.notes -r ssh://remote/home/user/.notes-storage
note edit someNote.md
note show someNote.md
note git push
```

---

```bash
note sync  # to automaticly pull and merge remote changes
```

> [!NOTE]
>
> You can also check out `man note` for documentation.


## Roadmap

* [ ] Graph building based on markdown links
* [X] ~~Lock-file~~
* [X] ~~Synchronization~~
* [X] ~~Search by notes~~
* [X] ~~Directories~~
* [X] ~~Tree of notes~~


<h1 align="center"><a href="#top">▲</a></h1>