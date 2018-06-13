# README

## Plantilla de LaTeX - CICESE

Plantilla de LaTeX no oficial para la elaboración del documento de tesis de
Maestría en Ciencias y Doctorado en Ciencias del CICESE (Centro de Investigación
Científica y de Educación Superior de Ensenada, Baja California, México). Muchas
de las modificaciones y adaptaciones fueron tomadas de la plantilla
[iTesis](https://github.com/panzerfausten/latex_template_cicese).


## Compilación

Para compilar el documento se debe usar [LuaLaTeX](http://www.luatex.org/). En
*NIX basta con crear un archivo `.latexmkrc` en el `$HOME` con la siguiente
información:

    $pdf_mode = 1;
    $pdflatex = 'lualatex -interaction=nonstopmode -synctex=1 %O %S';
    $clean_ext = 'bbl rel %R-blx.bib %R.synctex.gz';

y ejecutar en la terminal (o en el editor de preferencia) el `latexmk`.
