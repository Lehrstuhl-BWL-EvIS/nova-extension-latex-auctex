# nova-extension-latex-auctex
Taking AucTeX (https://www.gnu.org/software/auctex/) as starting point to prepare for a Nova extension for LaTeX typesetting.

Features rendering LaTeX editing particularly efficient in GNU Emacs/AucTeX are:

* Inserting sectioning commands via C-c C-s
* Inserting references from associated BibTeX files via RefTeX's cite commands (customizable to different \citeX commands such as \citep or \parencite)
* Inserting LaTeX environments such as \begin{itemize} ... \end{itemize) and inserting \item commands via ESC-m (hit ESC, then Return/Enter)
* Showing the table of contents with quick jump to a specific section via RefTeX's toc commands
* Run latexmk or pdflatex or lualatex depending on file-dependent variables 
* 
