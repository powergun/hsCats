# Category Theory and Python

## Visualization

jupyter does not natively support Latex tikz extension but someone
wrote a hack to bridge the gap: <https://github.com/mkrphys/ipython-tikzmagic>

to use this hack I need to `poetry add git+https://github.com/mkrphys/ipython-tikzmagic.git`
to install it from the repo

and also need to install the standalone latex debian package, and
pdf2svg package; image magick should have been installed at this point
but double check that as well: `convert --help`

<https://dzone.com/articles/installing-latex-ubuntu>

`sudo apt install pdf2svg`

once done, call `vis` to launch a **seperate jupyter nb process** that
has the tikz extension

note that i also need to set the output format `%%tikz -f svg` otherwise
it will fail silently

