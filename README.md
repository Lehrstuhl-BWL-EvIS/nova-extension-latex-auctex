# nova-extension-latex-auctex
Taking AucTeX (https://www.gnu.org/software/auctex/) as starting point to prepare for a Nova extension for LaTeX typesetting.

Features rendering LaTeX editing particularly efficient in GNU Emacs/AucTeX are:

* Inserting sectioning commands via C-c C-s
* Inserting references from associated BibTeX files via RefTeX's cite commands (customizable to different \citeX commands such as \citep or \parencite)
* Inserting LaTeX environments such as \begin{itemize} ... \end{itemize) and inserting \item commands via ESC-m (hit ESC, then Return/Enter)
* Outlining: Showing the table of contents with quick jump to a specific section via RefTeX's ToC commands
* Multi-file handling (\include{}) and corresponding file parsing 
* Run latexmk or pdflatex or lualatex depending on file-dependent variables 
* useful syntax color highlighting
* 
* ... 

Goal of this project is to recreate these features in an extension to [Nova.app](https://nova.app):

https://docs.nova.app/

https://docs.nova.app/extensions/

https://devforum.nova.app/

Currently, two extensions exist for Nova for editing LaTeX documents:

https://github.com/mava/nova-latex

https://github.com/flyx/Nova-TeX-Suite

Additionally, [TeXlab](https://github.com/latex-lsp/texlab) provides a cross-platform implementation of the Language Server Protocol providing rich cross-editing support for the LaTeX typesetting system including code completion. 
