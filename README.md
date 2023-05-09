# nova-extension-latex-auctex
Taking AucTeX (https://www.gnu.org/software/auctex/) as starting point to prepare for a Nova extension for LaTeX typesetting.

Features rendering LaTeX editing particularly efficient in GNU Emacs/AucTeX are:

* Inserting sectioning commands via C-c C-s
* Inserting references from associated BibTeX files via RefTeX's cite commands (customizable to different \citeX commands such as \citep or \parencite)
* Inserting LaTeX environments such as \begin{itemize} ... \end{itemize) and inserting \item commands via ESC-m (hit ESC, then Return/Enter)
* Outlining: Showing the table of contents with quick jump to a specific section via RefTeX's ToC commands
* Run latexmk or pdflatex or lualatex depending on file-dependent variables 
* ... 

Goal of this project is to recreate these features in an extension to [Nova.app](https://nova.app):

https://docs.nova.app/

https://docs.nova.app/extensions/

https://devforum.nova.app/

Es gibt bereits zwei Extensions für das Editieren von LaTeX-Dokumenten, die beide im Quellcode auf GitHub verfügbar sind:

https://github.com/mava/nova-latex

https://github.com/flyx/Nova-TeX-Suite


Im Rahmen einer Masterarbeit sollten, wie im Themenvorschlag erwähnt, u.a. folgende Features adressiert werden:

sinnvolles Syntax-Highlighting mit einem bewährten Farbmodell

Code-Completion - (via texlab : https://github.com/latex-lsp/texlab)

Code-Completion für BibTeX-Referenzen aus einem oder mehreren .bib-Dateien

Multi-File-Handling (bei Einbindung via \include{} )

diverse Keyboard-Shortcuts sinnvoll belegen (Liste käme von mir)

Outlining für umfangreiche LaTeX-Dokumente (schnelles Springen zwischen Kapiteln)


