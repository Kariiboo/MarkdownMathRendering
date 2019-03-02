# Markdown Preview Enhanced example
  
  
[Visual Studio Code](https://code.visualstudio.com ) and [Atom](https://atom.io ) have a [Markdown Preview Enhanced](https://shd101wyy.github.io/markdown-preview-enhanced ) extension that allows to render math & diagrams (UML, ...) inside the IDE and has export features, including HTML, PDF and markdown.
  
## Math
  
  
Markdown Preview Enhanced uses KaTeX or MathJax to render math expressions. 
  
Expression within `<img src="https://latex.codecogs.com/gif.latex?..."/>` or `<img src="https://latex.codecogs.com/gif.latex?..."/>` will be rendered inline.
Expression within `<p align="center"><img src="https://latex.codecogs.com/gif.latex?..."/></p>  
` or `<p align="center"><img src="https://latex.codecogs.com/gif.latex?..."/></p>  
` or ` ```math ` will be rendered in block.
  
See https://shd101wyy.github.io/markdown-preview-enhanced/#/math
  
```math
cos^2(\alpha) + sin^2(\alpha) = 1
```
  
<p align="center"><img src="https://latex.codecogs.com/gif.latex?tan(&#x5C;alpha)%20=%20&#x5C;frac%20{sin(&#x5C;alpha)}%20{cos(&#x5C;alpha)}"/></p>  
  
  
## Diagrams
  
  
Markdown Preview Enhanced supports rendering `flow charts`, `sequence diagrams`, `mermaid`, `PlantUML`, `WaveDrom`, `GraphViz`, `Vega` & `Vega-lite`, `Ditaa diagrams`.
  

![](assets/1fdaa2e0d2a717311dc056558dc0fed10.png?0.34705612409859343)  
See https://shd101wyy.github.io/markdown-preview-enhanced/#/diagrams
  
## Export in Github Flavor Markdown (GFM)
  
  
Markdown Preview Enhanced supports compilation into GitHub Flavored Markdown so that the exported markdown file will include all graphs (as png images), code chunks (hide and only include results), math typesettings (show as image) etc and can be published on GitHub.
See https://shd101wyy.github.io/markdown-preview-enhanced/#/markdown
  
Open the MPE preview: Commande Palette (<kbd>Ctrl-Shift-P</kbd>) > Markdown Preview Enhanced: Open Preview (<kbd>Ctrl + K V</kbd>). Then, on the preview, <kbd>right-click</kbd>, `Save as markdown`
  
Notes: 
- Math expressions are rendered as images using the latex.codecogs.com online service: `<img src="https://latex.codecogs.com/gif.latex?tan(&#x5C;alpha)%20=%20&#x5C;frac%20{sin(&#x5C;alpha)}%20{cos(&#x5C;alpha)}"/>`
- Diagrams are saved as png images to `imageFolderPath` (defaults to `/assets`). The exported image filename can be controlled by declaring {filename="your_file_name.png"}.
  