# Xovee's CV Template

[![Compile](https://github.com/Xovee/latex-cv/actions/workflows/compile.yml/badge.svg)](https://github.com/Xovee/latex-cv/actions/workflows/compile.yml)
[![Open in Overleaf](https://img.shields.io/badge/Overleaf-Open_as_Template-138A07?logo=overleaf)](https://www.overleaf.com/latex/templates/xovees-cv-template/rrsmqwhbygcf)

A clean, carefully structured LaTeX template for your academic CV. Easy to read, easy to update, and designed to grow with your work.

Designed and maintained by [Xovee Xu](https://www.xoveexu.com).

<p align="center">
  <a href="cv.pdf">
    <img src="example.png" width="600" alt="First-page preview of Xovee's CV Template. Click to view the complete PDF.">
  </a>
</p>

## Quick start

### Overleaf

Open the [published Overleaf template](https://www.overleaf.com/latex/templates/xovees-cv-template/rrsmqwhbygcf), select **Open as Template**, and edit the copy in your account.

The latest version is available on [GitHub](https://github.com/Xovee/latex-cv).

### Local LaTeX

Clone or download this repository and customize the template with your own information and content.

## File structure

| File | Purpose |
| --- | --- |
| `cv.tex` | Main document, identity values, contact block, and PDF metadata |
| `content.tex` | Fictional sample records to replace with your own content |
| `xovee-cv.sty` | Shared typography, spacing, entry environments, and helper commands |
| `cv.pdf` | Compiled example |

Keeping presentation rules in `xovee-cv.sty` makes global changes predictable. Ordinary CV updates should normally touch only `cv.tex` and `content.tex`.

## Layout and customization

Different types of CV content use layouts suited to how they are read:

| Content | Layout | Commands |
| --- | --- | --- |
| Publications, patents, and theses | Numbered citations | `\item` (in `enumerate`) |
| Funding and talks | Year at left, details aligned beside it | `\cvfundingitem`, `\cvtalkitem` |
| Education, appointments, awards, and teaching | Main entry at left, date at right, details below | `\cvdateditem`, `\cvdaterow` |
| Memberships, profiles, and service lists | Compact lists with aligned labels and details | `\cvmembershipitem`, `\cvregisterrow` |

To add an entry, copy a similar example in `content.tex` and replace its content. Add, remove, or reorder sections as needed.

For changes to fonts, spacing, or alignment throughout the CV, edit the shared definitions in `xovee-cv.sty`.

## Tips

- Tailor the CV to your needs and highlight what matters most.
- Less formatting is often more. Consistency is key.

Further reading: [Academic Job Search - CV (UC Berkeley)](https://career.berkeley.edu/grad-students-postdocs/academic-job-search/the-cv-part-1-overview/).

## Paper, font, and compilers

The default is A4 paper, 10-point Libertinus serif type, and one-inch margins. To use US Letter, change `a4paper` to `letterpaper` in `cv.tex`.

To use a different font, replace the `libertinus` package in `xovee-cv.sty` with your preferred font setup. See the [LaTeX Font Catalogue](https://tug.org/FontCatalogue/) for options.

The default template supports pdfLaTeX, XeLaTeX, and LuaLaTeX. The included PDF is compiled with pdfLaTeX.

## Publications and BibTeX

Publications are entered manually (my preferred approach) for full control and minimal dependencies. If you prefer BibTeX or `biblatex`, add a `.bib` file and the bibliography package of your choice; keep the citation ordering and visible fields consistent with the rest of the CV.

## Attribution

If you share a modified version of this template, a link back to [this repository](https://github.com/Xovee/latex-cv) is appreciated.

## License

[MIT](LICENSE)

## Contact

[Xovee Xu](https://www.xoveexu.com)

Email: `xovee.xu at gmail.com`

Suggestions and bug reports are welcome through [Issues](https://github.com/Xovee/latex-cv/issues). Contributions and improvements are welcome via [pull requests](https://github.com/Xovee/latex-cv/pulls).
