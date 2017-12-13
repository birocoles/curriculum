# Files

* `cv.tex`: Latex version of the CV.
* `cv.pdf`: PDF version of the CV.
* `cv.dbj`: Driver file to produce `cv.bst` from `merlin.mbs`. Generated with `makebst`.
* `cv.bst`: It defines a custom bibliographic style.
* `papers.bib`: List of peer-reviewed papers.
* `conferences.bib`: List of works presented at international conferences.

# Compiling the files

Execute the following steps, including the repeated ones:

    1. PDFLaTeX `cv.tex`
    2. BibTeX   `papers.bib`
    3. BibTeX   `conferences.bib`
    4. Comment the `\bibliography{papers}` command at the `papers.tex` file
    5. Copy the `papers.bbl` content and paste it at the end of the `papers.tex` file
    6. Comment the `\bibliography{conferences}` command at the `conferences.tex` file
    7. Copy the `conferences.bbl` content and paste it at the end of the `conferences.tex` file
    8. PDFLaTeX `cv.tex`
    9. PDFLaTeX `cv.tex`
