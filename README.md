# LaTeX Template for CU Boulder Graduate Theses

An improved version of CU Boulder's [original](https://www.colorado.edu/graduateschool/academic-resources/thesis-dissertation-specifications/thesis-dissertation-templates) LaTeX thesis template.  Updated to match the latest graduate school requirements, this template also includes a variety of other small improvements and capabilities as compared with the original.  A few notable improvements include:

- The base `thesis.tex` file now references lots of useful packages.
- _Italics_ are used instead of **boldface** to emphasize text (i.e., for the `\emph{}` command).  I confirmed with the graduate school that the [instructions](https://www.colorado.edu/graduateschool/sites/default/files/attached-files/latexthesisinstructions_2020.pdf), which require boldface, are out of date.
- Typesetting of footnotes is improved.
- Added `\introductoryPage`, `\titlePageTitle`, and `\thesisDirectedBy` commands.

See the changelog in `thesis.cls` for more details.

I submitted my physics [PhD dissertation](https://media.proquest.com/media/hms/PFT/2/7hwaR?_s=A2RkJg2HN1WqrgUA0fI4K213EXU%3D) to the graduate school using this template in May 2023.

## How To Use This Template

To use this template, clone or [download](https://github.com/GiacoCorsiglia/cu-boulder-thesis-template/archive/refs/heads/main.zip) this entire repository.  Your starting point for editing is the `thesis.tex` file.  You need to keep `thesis.cls` around, too, but you don't need to edit that file.

1. Set the title of your thesis and other details in the "PREAMBLE" section of `thesis.tex`.
2. Each chapter has its own folder and `.tex` file.  To add a new chapter, create `chapter-3/chapter.3.tex` and add it to the list of included chapters in the "CHAPTERS" section of `thesis.tex`
3. The same goes for appendices.
4. By default, it's expected that you'll manage your bibliography using BibTeX in the `bibliography.bib` file.  Check out "BIBLIOGRAPHY SETUP" in `thesis.tex` to customize this or to reference other `.bib` files.
5. If you organize your figures into folders, you must reference them using their full path relative to the root of the repository.  For example, a figure that lives in the `chapter-1` folder should be references as `chapter-1/fig.pdf`, otherwise LaTeX won’t find it.
6. If you have custom LaTeX command definitions to include, throw those in `macros.tex`.

See the `thesis.pdf` file for more tips on writing TeX in this template.
