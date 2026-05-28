cat > README.md <<'EOF'
# uothesis-memoir

A LaTeX dissertation/thesis template for the current University of Oregon ETD style, based on the 2023 style requirements from the Division of Graduate Studies.

This template is unofficial. It was developed by Yongmin Park, a PhD candidate in the Department of Mathematics at the University of Oregon.

## Overleaf Gallery

This template is also available on the Overleaf Gallery:

https://www.overleaf.com/latex/templates/uothesis-memoir/nnwbzcpckqhd

## Disclaimer

This is an unofficial University of Oregon thesis/dissertation LaTeX template.

It is not maintained, endorsed, or approved by the University of Oregon. Users are responsible for checking the template against the current UO Thesis and Dissertation Style and Policy Manual before submission.

## Template Structure

### main.tex

This is the main file to compile in order to generate the document.

It contains only the skeleton of the dissertation/thesis. The preamble, prefatory material, and main body are separated into different `.tex` files.

The structure is roughly:

1. Declare the document class.
2. Load `packages.tex`.
3. Load `preamble-after-pkg.tex`.
4. Declare the dissertation/thesis information.
5. Begin the document.
6. Load `prefatory.tex`.
7. Load the main body from `Text-tex/`.
8. End the document.

### uothesis-memoir.sty

This is the package file for the dissertation/thesis template.

It contains the commands required for styling the document. The file is intentionally kept minimal, so most users should be able to modify the document without making many changes here.

### packages.tex

This file contains the package-loading commands.

Some useful packages are already loaded. Be careful not to load duplicate packages. Also note that the loading order matters for some packages. If you add, remove, or change packages, please refer to the relevant package documentation on CTAN.

### preamble-after-pkg.tex

This file contains the part of the preamble that is loaded after the packages.

It includes custom commands and the bibliography setup.

### prefatory.tex

This file typesets the prefatory pages.

It mainly loads the corresponding `.tex` files from `prefatory-tex/`.

### biblatex.cfg

This file defines an AMS-like `biblatex` style.

If you want to change the citation or bibliography style, you may need to modify or remove this file.

### biblatex-note.txt

Notes on using `biblatex`.

### bib.bib

This is the sample bibliography file.

You may either modify this file for your own bibliography or use your own `.bib` file. If you use a different bibliography file, load it in `preamble-after-pkg.tex`.

### changelog.txt

The changelog for each version of the template.

### prefatory-tex/

This folder contains the `.tex` files for the prefatory pages.

You should modify the following files for your dissertation/thesis:

- `abstract.tex`
- `ack-ded.tex`
- `copyright.tex`
- `cv.tex`
- `title.tex`

Please refer to the comments in each file.

### Text-tex/

This folder contains the `.tex` files for the main body of the dissertation/thesis.

Because of the ETD style requirements, appendices are typeset differently depending on whether the document has a single appendix chapter or multiple appendix chapters.

## License

This project is licensed under the LaTeX Project Public License, version 1.3c.
EOF
