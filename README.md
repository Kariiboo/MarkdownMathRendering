# Math rendering in GitHub markdown

The GitHub's markdown doesn't support math rendering.
Math expressions have to be rendered as images before being included in GitHub markdown files

## Offline pre-rendering solution

[Visual Studio Code](https://code.visualstudio.com) and [Atom](https://atom.io) have a [Markdown Preview Enhanced](https://shd101wyy.github.io/markdown-preview-enhanced) extension that allows to use math expressions and diagrams (UML, graphviz, ...) in markdown, inside the IDE and export that markdown to a Github Flavor Markdown.

The `MPE_example.md` page has been saved as markdown [here](MPE_example_.md)

* Pro: Math + diagrams + code chunk support.
* Cons: Math expression rendering is of poor quality once saved as markdown (due to the use of GIF images https://latex.codecogs.com/gif.latex?...). [Issue opened](https://github.com/shd101wyy/vscode-markdown-preview-enhanced/issues/189).

## Online rendering solution

TeXify is a GitHub App that looks in git pushes for files with extension *.tex.md and renders it's TeX expressions as SVG images.
It supports TeX rendering only. No diagrams. It can be used easily when editing files online on github web site.

TeXify GitHub App is installed on this GitHub repository.
The `TeXify_example.tex.md` page in this repository is then automatically processed on git pushes to generate [this page](TeXify_example.md)

* Pro: Math expression rendering is of good quality.
* Cons: Only Math support, no diagrams, no code chunk support.

## Bibliography

- Markdown Preview Enhanced: https://shd101wyy.github.io/markdown-preview-enhanced
- "Latex rendering in `README.md` on Github" question on stackoverflow :  https://stackoverflow.com/questions/35498525/latex-rendering-in-readme-md-on-github and this answer https://stackoverflow.com/questions/35498525/latex-rendering-in-readme-md-on-github/53981118#53981118
