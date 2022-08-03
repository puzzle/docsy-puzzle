# Docsy Puzzle

Additions for the [docsy theme](https://github.com/google/docsy) for [Hugo](https://gohugo.io/), used for [Puzzle](https://puzzle.ch/) training content.
The docsy-puzzle theme inherites from the docsy theme through Hugo [Modules](https://gohugo.io/hugo-modules/use-modules/).

The theme adds the following to the standard docsy theme:

* Puzzle ITC colors scheme and fonts
* Puzzle ITC logo

## Installation

To add the [docsy](https://github.com/google/docsy), [docsy-plus](https://github.com/puzzle/docsy-plus) and docsy-puzzle themes to an existing Hugo project, run the following commands from your project’s root directory:

```sh
hugo mod get github.com/acend/docsy-plus
hugo mod get github.com/puzzle/docsy-puzzle
```

Reference both themes in your configuration, the docsy-puzzle theme needs to come before docsy.

Example config.toml:

```toml
[module]
  [module.hugoVersion]
    extended = true
    min = "0.100.0"
  [[module.imports]]
    path = "github.com/puzzle/docsy-puzzle"
    disable = false
  [[module.imports]]
    path = "github.com/acend/docsy-plus"
    disable = false
```

Docsy itself is a dependencsy of docsy-plus