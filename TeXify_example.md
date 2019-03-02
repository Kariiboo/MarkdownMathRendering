# TeXify example

TeXify is a GitHub App that looks in git pushes for files with extension *.tex.md and renders it's TeX expressions as SVG images.
It support TeX rendering only. No diagrams. It can be used easily when editing files online on github web site.

It generate a tex folder that contains all generated files.
The TeXify GitHub App works only at git push. Once the markdown is generated, it can even be uninstalled from the repository.

See also: https://github.com/kamil-kielczewski/fractals

## Math

Expression within \$...\$ or will be rendered inline.

* <img src="/tex/f263f13eee056a0618d09cebb820fe15.svg?invert_in_darkmode&sanitize=true" align=middle width=157.723731pt height=26.76175259999998pt/>
* <img src="/tex/ce4098d166c6b2204133b66304cbd215.svg?invert_in_darkmode&sanitize=true" align=middle width=109.5455262pt height=33.20539859999999pt/>

Expression within \$\$...\$\$ will be rendered in blocks.
  
<p align="center"><img src="/tex/638934f72067a7dc5332ce0465e4c458.svg?invert_in_darkmode&sanitize=true" align=middle width=157.723731pt height=18.312383099999998pt/></p>
<p align="center"><img src="/tex/51091157aa7daeb97c96fff0deaa2dd5.svg?invert_in_darkmode&sanitize=true" align=middle width=118.34180159999998pt height=38.83491479999999pt/></p>
<p align="center"><img src="/tex/b676777fa34e0c8748b5fd33866e35e1.svg?invert_in_darkmode&sanitize=true" align=middle width=288.09219945pt height=16.438356pt/></p>