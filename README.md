# Isidro Butaslac III, PhD - Academic CV

This CV reflects my academic journey.

## Download

![Workflow name](https://github.com/sid410/Butaslac-CV/actions/workflows/latex_build.yml/badge.svg?branch=main)

Changes are automatically updated with CI/CD, and the latest version is always accessible through the following link:

https://github.com/sid410/Butaslac-CV/releases/download/latest-release/butaslac_cv.pdf

## How to Compile

This CV is compiled using `pdflatex`, ensuring wide compatibility and easy reproduction of the document.

To compile the CV from source with local LaTeX environment:
1. Install `texlive-full`
2. Run the following command in your terminal:

   ```bash
   pdflatex -output-directory=build butaslac_cv.tex
   ```

To compile the CV from source with Docker:
1. The project uses `texlive/texlive` Docker container for compilation.
2. Run the following command in your terminal:

   ```bash
   docker run --rm -v $PWD:/workdir texlive/texlive pdflatex -output-directory=/workdir/build /workdir/butaslac_cv.tex
   ```
