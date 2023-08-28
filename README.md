# nova-extension-latex-auctex
Taking AucTeX (https://www.gnu.org/software/auctex/) as starting point to prepare for a Nova extension for LaTeX typesetting.

Features rendering LaTeX editing particularly efficient in GNU Emacs/AucTeX are (but need more ergonomic keybindings in Nova!):

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


## Requirements (by priority)

- via keyboard / mouse-free: Create a table of contents (TOC) in a sidebar showing all sections of the document and allow for quick jumping to a section via keybindings, i.e., press a key to show TOC (in sidebar) and then navigate TOC via arrow keys and hit return/enter to jump to section under cursor
- Support multi-file documents, i.e., evaluate the \include and \input commands
- via keyboard / mouse-free: Insert sectioning commands \chapter, \section etc. (possibly via texlab LSP)
- via keyboard / mouse-free: Insert references from associated BibTeX files via RefTeX's cite commands, possibly customizable to different \citeX commands such as \citep (for natbib) or \parencite (for BibLaTeX)
- via keyboard / mouse-free:  Insert LaTeX environments such as \begin{itemize} ... \end{itemize) and inserting \item commands via ESC-m (hit ESC, then Return/Enter)
- Run (La)TeX engine without running latexmk (i.e., .latexmkrc) by evaluating well-known meta commends in comments, see https://tex.stackexchange.com/questions/78101/when-and-why-should-i-use-tex-ts-program-and-tex-encoding
- Support folding and unfolding of parts of the LaTeX source at the level of \chapter, \section, and \subsection to allow for concentrating on current part of document, see https://www.gnu.org/software/auctex/manual/auctex/Folding.html

## Related work

Currently, two extensions exist for Nova for editing LaTeX documents:

https://github.com/mava/nova-latex

https://github.com/flyx/Nova-TeX-Suite

Additionally, [TeXlab](https://github.com/latex-lsp/texlab) provides a cross-platform implementation of the Language Server Protocol providing rich cross-editing support for the LaTeX typesetting system including code completion. 

Then, of course, AucTeX : https://www.gnu.org/software/auctex/

## Foundations

- Text editor (as a class of software)
- Text editing (as a task, as a mode of usage of text editor software)
- LaTeX text editing, i.e., editing (non-trivial) LaTeX documents
- General text editing ergonomics, see, e.g.,
  - Apple Human Interface Guidelines : https://developer.apple.com/design/human-interface-guidelines
  - alternative keyboard layouts, e.g., Dvorak, Maltron, Colemak, Neo, [adnw](http://www.adnw.de)
- Research on user interface ergonomics in general and user input / keyboard / mouse ergonomics in particular
- Research on editing large text documents
- Research on editing large LaTeX documents
- Research on writer productivity

## Installation

The TypeScript files can be transpiled to JavaScript with `npm run build`.
