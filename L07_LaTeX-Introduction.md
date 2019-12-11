# Introduction to scientific working

## Writing scientific document

Writing a scientific document can be done with several tools.
From simple text pages written in a text processor like _Microsoft Word_,
_Libreoffice Writer_ or _Google Docs_ to specialized tools.

Which tool to use depends often on the branch of science an author and research
can be seen as part of.

Where in humanitie-science like psycology, literature, philosophy and others it
is more common to write a scientific document in a word processor.
In nature sciences like physics, informatics, mechanics it is more common to use
technical systems like _LaTeX_ to write documents.

The need for specialized tools in nature sciences is rooted in the needs to
write formulas, tables, citations, graphs, data includes and other material
without the requirement of the user to specify the visual style every time.

And to be able to use the same written content in different documents without
reapplying a changed visual style.

### What is LaTeX?

LaTeX is an extension to the TeX document preparation system.
It uses plain-text files with annotated passages in it and a processor.

It is also further extensible with packages to draw circuits, graphs and other
types needed in books or scientific documents.

### How to write a document with LaTeX

A document written in LaTeX is starting with the definition of type of document.
The `documentclass` initializes defaults for styles and structure marker.
It can define structure of a title page, page numbers, head lines, foot notes
and much more.

These styles are consistently applied to the complete content of the document
without the need of the author to take care of it.

**Example:**

```LaTeX
    \documentclass{article}
    \usepackage{amsmath}
    \title{\LaTeX}

    \begin{document}
      \maketitle
      \LaTeX{} is a document preparation system for
      the \TeX{} typesetting program. It offers
      programmable desktop publishing features and
      extensive facilities for automating most
      aspects of typesetting and desktop publishing,
      including numbering and  cross-referencing,
      tables and figures, page layout,
      bibliographies, and much more. \LaTeX{} was
      originally written in 1984 by Leslie Lamport
      and has become the  dominant method for using
      \TeX; few people write in plain \TeX{} anymore.
      The current version is \LaTeXe.

      % This is a comment, not shown in final output.
      % The following shows typesetting  power of LaTeX:
      \begin{align}
        E_0 &= mc^2 \\
        E &= \frac{mc^2}{\sqrt{1-\frac{v^2}{c^2}}}
      \end{align} 
    \end{document}
```

### How to use LaTeX on ...?

The most known and complete distribution/collection of tools and packages for
LaTeX is <a href="https://miktex.org" target="_blank">MiKTeX</a>, it is
available for _Microsoft Windows_, _macOS_, _Linux_.

There are also some graphical user interface tools:
_(this is a small list and not to be considered comprehensive or a
recommendation list)_

- [TeXstudio](https://www.texstudio.org)
- [LyX](https://www.lyx.org)
- [TeXMaker](https://www.xmlmath.net/texmaker)
- [Gummi](https://github.com/alexandervdm/gummi) _Linux/BSD only_
- [TeXpen](https://sourceforge.net/projects/texpen)
- [Overleaf](https://www.overleaf.com) _Online Editor with collaboration
  support_

And of course LaTeX is able to be used on a command line.

_(My favorite:
NeoVim with plugins: `ncm2`, `ale` \[with latex linter\], `vimtex`.
But I do nearly everything in vim 😉 )_

### Next:

[LaTeX Document Classes](L08_LaTeX-Document-Classes.md)
