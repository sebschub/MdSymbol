MdSymbol - A math symbol font
=============================

MdSymbol is a math symbol font, designed as a companion to Myriad Pro
by Adobe, but it might also fit other contemporary typefaces. MdSymbol
is based on FdSymbol by Michael Ummels released under the [SIL Open
Font License][OFL], Version 1.1.


Usage
-----

To use this font in LaTeX, include

    \usepackage{mdsymbol}

in the preamble of your LaTeX document. See the PDF documentation for
the details.

Installation
------------

Building the fonts requires Metafont (>=2.718281), MetaPost (>=1.211),
mf2pt1 (>= 2.4.4), FontForge (>=20110222), and Python 2.7 with the fontforge
module enabled.

To install the fonts, the accompanying LaTeX package and the documentation
in your home texmf tree, run:

    make install

If you want to use a different texmf tree, you can specify it using the
variable TEXMFDIR:

    make install TEXMFDIR=/usr/local/texlive/texmf-local

Afterwards, you may need to regenerate the file database:

    texhash

Finally, you need to activate the map file:

    updmap --enable Map=mdsymbol.map

For a system-wide installation, replace updmap by updmap-sys.

License
-------

Copyright (c) 2011 by Sebastian Schubert <schubert.seb@googlemail.com>

The font components of this software, e.g. MetaFont (.mf), TeX font metric
(.tfm), Type 1 (.pfb), and OpenType (.otf) files, are licensed under the
[SIL Open Font License][OFL], Version 1.1.

[OFL]: http://scripts.sil.org/OFL

The LaTeX support files contained in this software may be modified and
distributed under the terms and conditions of the
[LaTeX Project Public License][LPPL], version 1.3c or greater (your choice).

[LPPL]: http://www.latex-project.org/lppl/

This work has the LPPL maintenance status `maintained'.

The Current Maintainer of this work is Sebastian Schubert.

This work consists of the files mdsymbol.dtx, mdsymbol.ins
and the derived files mdsymbol.sty and mdsymbol.pdf.

All other files distributed with these sources, e.g. the Makefile and
the Python scripts were written by Michael Ummels and are in the
public domain.
