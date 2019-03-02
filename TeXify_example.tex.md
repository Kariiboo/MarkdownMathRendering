# TeXify example

TeXify is a GitHub App that looks in git pushes for files with extension *.tex.md and renders it's TeX expressions as SVG images.
It support TeX rendering only. No diagrams. It can be used easily when editing files online on github web site.

It generate a tex folder that contains all generated files.
The TeXify GitHub App works only at git push. Once the markdown is generated, it can even be uninstalled from the repository.

TeXify GitHub App is installed on this GitHub repository.
The `TeXify_example.tex.md` page of this repository is then automatically processed on git push to generate [this page](TeXify_example.md)

See also: https://github.com/kamil-kielczewski/fractals

## Math

Expression within `$...$` or will be rendered inline.

* $cos^2(\alpha) + sin^2(\alpha) = 1$
* $tan(\alpha) = \frac {sin(\alpha)} {cos(\alpha)}$

Expression within `$$...$$` will be rendered in blocks.
  
$$cos^2(\alpha) + sin^2(\alpha) = 1$$
$$tan(\alpha) = \frac {sin(\alpha)} {cos(\alpha)}$$
$$cos(a + b) = cos(a) cos(b) - sin(a)sin(b)$$