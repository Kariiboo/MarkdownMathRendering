# Math rendering in GitHub markdown

The GitHub markdown doesn't support math rendering.
Math expressions have to be rendered as images before being included in markdown files

## Offline pre-rendering solution

[Visual Studio Code](https://code.visualstudio.com) and [Atom](https://atom.io) have a [Markdown Preview Enhanced](https://shd101wyy.github.io/markdown-preview-enhanced) extension that allows to render math & diagrams (UML, ...) inside the IDE and export as Github Flavor Markdown.

The `MPE_example.md` page has been saved as markdown [here](MPE_example_.md)

* Pro: Math + diagrams + code chunk support.
* Cons: Math expression rendering poor quality (due to the use of https://latex.codecogs.com/)

## Online rendering solution

TeXify is a GitHub App that looks in git pushes for files with extension *.tex.md and renders it's TeX expressions as SVG images.
It support TeX rendering only. No diagrams. It can be used easily when editing files online on github web site.

TeXify GitHub App is installed on this GitHub repository.
The `TeXify_example.tex.md` page of this repository is then automatically processed on git push to generate [this page](TeXify_example.md)

* Pro: Math expression rendering good quality.
* Cons: Only Math support, no diagrams, no code chunk support.

## Bibliography

- Markdown Preview Enhanced: https://shd101wyy.github.io/markdown-preview-enhanced
- "Latex rendering in `README.md` on Github" question on stackoverflow :  https://stackoverflow.com/questions/35498525/latex-rendering-in-readme-md-on-github and this answer https://stackoverflow.com/questions/35498525/latex-rendering-in-readme-md-on-github/53981118#53981118