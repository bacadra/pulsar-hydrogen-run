# hydrogen-run

![hydrogen-run](https://github.com/bacadra/hydrogen-run/blob/master/assets/hydrogen-run.gif?raw=true)

The package extends the available methods to computing with [hydrogen](https://github.com/nteract/hydrogen).

## Installation

After the announcement of Atoms sunset, the official [Atom packages store](https://atom.io/packages) isn't respond properly, so latest version of this package cannot be downloaded there. To get latest version run the shell command

    apm install bacadra/atom-hydrogen-run

and obtain the package directly from Github repository. Please note that package will occur in `Settings/Packages/Git Packages` instead of `Community Packages`.

## New concepts

The package introduce two new concepts of evaluation:

* `recalculate`: clear result + restart kernel + run calculation,
* `inline`: computing go one breakpoint after one (instead of pushing all text to python interpreter instantly), this way you got result next to breakpoints. Inline methods inherit all limitations of hydrogen package, e.g. in python the block `if ... else ...` need to be extended, but it's not.

## List of commands

The commands have been assigned to the function keys with optional modifier keys. There are few method from [hydrogen](https://github.com/nteract/hydrogen) package which have been assigned too.

| Shortcut | Command | Description |
| -: | - | - |
| `F5` | `hydrogen:run-all` | push all text in single run; standard method of Hydrogen |
| `Alt-F5` | `hydrogen-run:recalculate-all` | clear results, reset kernel and push all text in single run |
| `Shift-F5` | `hydrogen:run-all-above` | push above text in single run |
| `Ctrl-F5` | `hydrogen-run:recalculate-all-above` | clear results, reset kernel and push above text in single run |
| `F6` | `hydrogen-run:run-all-inline` | push all text in multiple runs |
| `Alt-F6` | `hydrogen-run:recalculate-all-inline` | clear results, reset kernel and push all text in multiple runs |
| `Shift-F6` | `hydrogen-run:run-all-above-inline` | push above text in multiple runs |
| `Ctrl-F6` | `hydrogen-run:recalculate-all-above-inline` | clear results, reset kernel and push above text in multiple runs  |
| `F7` | `hydrogen:run` | run single statement in single run |
| `Ctrl-F7` | `hydrogen:run-cell` | run cell in single run |
| `Alt-F7` | `hydrogen:clear-and-center` | clear results and scroll text editor to cursor |
| `Shift-F7` | `hydrogen:interrupt-kernel` | interrupt kernel |
| `F8` | `hydrogen:run-and-move-down` | run single statement and go to next statement |
| `Ctrl-F8` | `hydrogen:run-cell-and-move-down` | run single cell and go to next cell |
| `Alt-F8` | `hydrogen-run:clear-and-restart` | clear results and restart kernel |
| `Shift-F8` | `hydrogen:shutdown-kernel` | shutdown kernel |
| `F9` | `hydrogen:toggle-inspector` | toggle inspector pane |

# Contributing

If you have ideas on how to improve the package, see bugs or want to support new features, feel free to share them via GitHub.

See my other packages dedicated to Atom Editor:

* [autocomplete-sofistik](https://github.com/bacadra/atom-autocomplete-sofistik)
* [bib-finder](https://github.com/bacadra/atom-bib-finder)
* [hydrogen-run](https://github.com/bacadra/atom-hydrogen-run)
* [image-paste](https://github.com/bacadra/atom-image-paste)
* [language-sofistik](https://github.com/bacadra/atom-language-sofistik)
* [navigation-panel](https://github.com/bacadra/atom-navigation-panel)
* [open-external](https://github.com/bacadra/atom-open-external)
* [pdf-viewer](https://github.com/bacadra/atom-pdf-viewer)
* [project-files](https://github.com/bacadra/atom-project-files)
* [regex-aligner](https://github.com/bacadra/atom-regex-aligner)
* [sofistik-tools](https://github.com/bacadra/atom-sofistik-tools)
* [super-select](https://github.com/bacadra/atom-super-select)
* [word-map](https://github.com/bacadra/atom-word-map)
