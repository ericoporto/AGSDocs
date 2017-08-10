# AGS Docs

This is a work in progress, this repository will at some point store a fork of the Adventure Game Studio Documentation,
[you can read it here](Markdown/ags.md).

You can [read in a webpage here](http://ericoporto.github.io/AGSDocs).


## Building the documentation

The docs should be written in Markdown, inside the Markdown folder.

When updated, just run the script `make_html_docs.sh`.

This script is temporary, soon documentation will be migrated to ReStructured
Text only since the support for it in Sphinx is better.


## How it works

This script will create rst files, place them in the `source` folder and then
fix the links (switching .md to .html) and then it will use **Sphinx** to
generate the html files. The html files are going to be used in the webpage.

After it will use **Sphinx** again to generate the QtHelp file to be used inside
FGMK itself.


# Dependencies

The script requires: sphinx, sphinx_rtd_theme (both on python3) and pandoc
installed.
