# TreeView

[![Build Status](https://travis-ci.org/dpsanders/TreeView.jl.svg?branch=master)](https://travis-ci.org/dpsanders/TreeView.jl)

[![Coverage Status](https://coveralls.io/repos/dpsanders/TreeView.jl/badge.svg?branch=master&service=github)](https://coveralls.io/github/dpsanders/TreeView.jl?branch=master)

[![codecov.io](http://codecov.io/github/dpsanders/TreeView.jl/coverage.svg?branch=master)](http://codecov.io/github/dpsanders/TreeView.jl?branch=master)


This is a small package to visualize a graph corresponding to an
abstract syntax tree (AST) of a Julia expression. It uses the `TikzGraphs.jl`
package to do the visualization.

## Usage

The package is designed to be used within the IJulia notebook.

The simplest usage is `@tree <EXPRESSION>`, where `<EXPRESSION>` represents any
Julia expression, for example
```
@tree x^2 + y^2
```
which gives the following output:

![example_tree](example_tree.png)

See [this notebook](examples/TreeView.ipynb) for usage examples.

## Author

- [David P. Sanders](http://sistemas.fciencias.unam.mx/~dsanders),
Departamento de Física, Facultad de Ciencias, Universidad Nacional Autónoma de México (UNAM)

## Acknowledements
Financial support is acknowledged from DGAPA-UNAM PAPIME grants PE-105911 and PE-107114, and DGAPA-UNAM PAPIIT grant IN-117214, and from a CONACYT-Mexico sabbatical fellowship. The author thanks Alan Edelman and the Julia group for hospitality during his sabbatical visit.

In particular, he thanks Jiahao Chen, who, when asked if a package like this existed,
replied "why don't you write one?".
