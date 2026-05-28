---- Description ----
This is a dissertation/thesis template for the current ETD (2023) style from Division of Graduate Studies of University of Oregon. This template is not official and developed by Yongmin Park, a PhD candidiate at the Department of Mathematics of University of Oregon.


---- Structure of the template ---

./main.tex
You need to compile this file to generate the document. Note that it only contains the skeleton of the whole documents. All the preambles and main body should be typed in different tex files. It is structured as

    Declare the document class;
    Load ./packages.tex;
    Load ./preamble-after-pkg.tex;
    Declare the dissertation/thesis information;
    Begin document;
        Load ./prefatory.tex
        Load main body of the document located in ./Text-tex/
    End document;

./uothesis-memoir.sty
The package file for this dissertation template. It contains all the commands required for the stylying the document. It is very minimal, so when you want to modify some style, typically, there will be no trouble without changing some commands in this file.

./packages.tex
It contains all the commands loading packages. Already some useful packages are loaded, so be careful so that you do not load duplicated packages. Moreover, for some packages, the order of loading is important, so if you want to add/change some packages here, please refer to the package documentation from CTAN.

./preamble-after-pkg.tex
This is the preamble part AFTER loading packages. It contains custom commands and loading bibliography file.

./prefatory.tex
This is for typesetting the prefatory pages. In only loads the corresponding tex files for the prefatory pages.

./biblatex.cfg
This is for the AMS-like BibLaTex style. If you want to change the citation and bibliography styles, you might change/remove this file.

./biblatex-note.txt
For some notes on using BibLaTex.

./bib.bib
The sample bibliography file. You may modify this file to adjust to your bibliography, or you can use own your bib file. In that case, please load your bib file in preamble-after-pkg.tex

./changelog.txt
For the change log of each version.

./prefatory-tex/
This folder contains all the tex files for typesetting the prefatory pages. You should modify 
    abtract.tex, ack-ded.tex, copyright.tex, cv.tex, title.tex
for your dissertation/thesis. Please refer to the comments for each file.

./Text-tex/
This folder contains the tex fiels for the main body. Because of the requirement from the ETD style, the appendix/appendices will be differently typeset according to whether you have a single appendix chapter or multiple appendix chapters. 





        
## Overleaf Gallery

This template is also available on the Overleaf Gallery:

https://www.overleaf.com/latex/templates/uothesis-memoir/nnwbzcpckqhd

## Disclaimer

This is an unofficial University of Oregon thesis/dissertation LaTeX template.

It is not maintained, endorsed, or approved by the University of Oregon. Users are responsible for checking the template against the current UO Thesis and Dissertation Style and Policy Manual before submission.

## License

This project is licensed under the LaTeX Project Public License, version 1.3c.
