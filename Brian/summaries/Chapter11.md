Chapter 11 Presenting with Latex
===========================================

## What is Latex?

LaTeX is a document preparation system and document markup language. It is the standard for the communication and publication of scientific documents. LaTeX uses the TeX typesetting program for formatting its output, and is itself written in the TeX macro language.  Almost any editing program or word-processor may be used to write LaTeX documents, although there are many editing programs written specially to make using LaTeX easy. 

LaTeX is widely used in academia. It is also used as the primary method of displaying formulas on many websites . LaTeX can be used as a primary or intermediate format, e.g., translating DocBook and other XML-based formats to PDF. The typesetting system offers programmable desktop publishing features and extensive facilities for automating most aspects of typesetting and desktop publishing, including numbering and cross-referencing, tables and figures, page layout and bibliographies.

### Should you use LaTeX?

Being able to use LaTeX properly is equivalent to saying that "It'll take a lot of work". There a few reasons for not attempting to use LaTeX. You shouldn't use LaTeX if

- You don't have time to learn it. Unlike most other point-and-click systems, LaTeX does take some time to learn. There are of course many guides and tutorials that can help you with this, but don't try to learn LaTeX if you have, say, less than 24 hours to prepare a manuscript.

- Your document is already written. Say, if you have already written your thesis in Word, there isn't much point in trying to "convert" your document to LaTeX. You can do it, but the results won't be pretty. LaTeX isn't just another "format" to store documents, it's a "system" to help you write those documents.

- All you care about is the design of the document. If you do care about creating your own designs for your documents (rather than the content), LaTeX is perhaps not the best system for you. There are a number of packages that allow you to customize the look of your document, but things are not always straightforward.

### What is the advantages of using Latex?

One of the advantages of LaTeX over other more traditional systems (e.g. Word or OpenOffice) is the high typographical quality of the documents that one will be able to produce. This is particularly true for documents that are heavy on mathematics, but documents for any other area could also take advantage of these qualities.

Since LaTeX is fully integrated with R, visual presentations of research can be produced and automatically updated with very little extra effort. This would greatly enhance the reproducibility of certain research. 

A less obvious advantage, but much more important, is that LaTeX allows the writer to clearly separate the content from the format of the document. This gives the writer the opportunity to focus on the "what", the creative part of the work, rather than the "how" is it going to look printed out in paper (that is the work of LaTeX document class designers).

## The Basics

Every LaTeX document follows the same general format, including a preamble and a body. The preamble goes at the beginning of the document, usually following the command `\documentclass`. The preamble specifies the global format for the entire document, including options and packages to be used. The body, contained between the commands `\begin{document}` and `\end{document}`, is where the content of the document is being created. 

### Basic commands

#### Headings

Section and subsection headings are automatically numbered and formatted by LaTeX. The basic syntax for specifying a section is `\section{section-name}`. There are a number of sub-section level headings, including `subsection`, `subsubsection`, `paragraph`, and `subparagraph`. To have an unnumbered section, use an asterisk (\*) in the command like this: `\section*{unnumbered}`.

#### Spacing

LaTeX automatically adjust spaces between paragraphs depending on document class. If more space is needed between certain paragraphs or lines, use the command `vspace{unit}`. Spacing unit can be any measurement unit, such as **cm, pt, em**, etc. If more horizontal space is needed, us the command `hspace`.

#### Text format

- **Italics & Bold** Use `\emph{}` or `\textit{}` to italicize text. Use `\textbf{}` to make text bold. We can also use both command concurrently to make text both bold and italicized; for example, `\textbf{\emph{some text}}`.
- **Font sizes** Font size can be set globally in the `documentclass` option, e.g., `\documentclass[12pt]{article}`. Body text sizes can also be formatted locally by using command such as `\Large` or `\small`.
