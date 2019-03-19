# Markdown Preview Enhanced example
  
  
[Visual Studio Code](https://code.visualstudio.com ) (and [Atom](https://atom.io )) have a [Markdown Preview Enhanced](https://shd101wyy.github.io/markdown-preview-enhanced ) (MPE) extension that allows to render math expressions & diagrams (UML, ...) inside the IDE and to export as GitHub Flavor Markdown (GFM).
  
## Math examples
  
  
Markdown Preview Enhanced render math expressions using :
* KaTeX or MathJax in embedded Markdown preview.
* https://latex.codecogs.com on line service for `Save as markdown` (export to GFM)
  
Expression within \$...\$ will be rendered inline.
  
* <img src="https://latex.codecogs.com/svg.latex?cos^2(&#x5C;alpha)%20+%20sin^2(&#x5C;alpha)%20=%201" style="vertical-align: middle;"/>
* <img src="https://latex.codecogs.com/svg.latex?tan(&#x5C;alpha)%20=%20&#x5C;frac%20{sin(&#x5C;alpha)}%20{cos(&#x5C;alpha)}" style="vertical-align: middle;"/>
  
Expression within \$\$...\$\$ will be rendered in blocks.
  
<p align="center"><img src="https://latex.codecogs.com/svg.latex?cos^2(&#x5C;alpha)%20+%20sin^2(&#x5C;alpha)%20=%201"/></p>  
  
<p align="center"><img src="https://latex.codecogs.com/svg.latex?tan(&#x5C;alpha)%20=%20&#x5C;frac%20{sin(&#x5C;alpha)}%20{cos(&#x5C;alpha)}"/></p>  
  
  
See https://shd101wyy.github.io/markdown-preview-enhanced/#/math
  
  
## Diagrams examples
  
  
Markdown Preview Enhanced supports rendering `flow charts`, `sequence diagrams`, `mermaid`, `PlantUML`, `WaveDrom`, `GraphViz`, `Vega` & `Vega-lite`, `Ditaa diagrams`.
  

![](assets/b0076a58206ea9e97ffaf61a14419cd90.png?0.5386068054621245)  
See https://shd101wyy.github.io/markdown-preview-enhanced/#/diagrams
  
## About `Save as markdown` (export to GFM)
  
  
Markdown Preview Enhanced supports compilation into GitHub Flavored Markdown so that the exported markdown file will include all graphs (as PNG images), code chunks (hide and only include results), math expressions (show as images) etc and can be published on GitHub.
See https://shd101wyy.github.io/markdown-preview-enhanced/#/markdown
  
Open the MPE preview: Commande Palette (<kbd>Ctrl-Shift-P</kbd>) > Markdown Preview Enhanced: Open Preview (<kbd>Ctrl + K V</kbd>). Then, on the preview, <kbd>right-click</kbd>, `Save as markdown`
  
__Notes__ :
  
- By default, math expressions are rendered as GIF images, using the latex.codecogs.com online service, like this: `<img src="https://latex.codecogs.com/gif.latex?tan(&#x5C;alpha)%20=%20&#x5C;frac%20{sin(&#x5C;alpha)}%20{cos(&#x5C;alpha)}"/>`. The images quality is not optimal and they don't scale up.
  But, since MPE v0.3.13, images format can be configured in settings : `File` > `Preferences` > `Settings` > `Extensions` > `Markdown Preview Enhanced` > `Math Rendering Online Service`. Consider using SVG (`https://latex.codecogs.com/svg.latex`) to have a better image quality that scale up.
- Diagrams are saved as PNG images to `imageFolderPath` (defaults to `/assets`). The exported image filename can be controlled by declaring {filename="your_file_name.png"}.
  