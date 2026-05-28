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

### `main.tex`

This is the main file to compile in order to generate the document.

It contains only the skeleton of the dissertation/thesis. The preamble, prefatory material, and main body are separated into different `.tex` files.

The structure is roughly:

```text
Declare the document class
Load packages.tex
Load preamble-after-pkg.tex
Declare dissertation/thesis information

Begin document
    Load prefatory.tex
    Load the main body from Text-tex/
End document
