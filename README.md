# Boolean Iteration

[Presentation](/presentation/iteration.md) on Loops and Iteration for [Boolean](https://boolean.co.uk/).

## Install

To recreate the html slideshows from the source [Markdown](https://en.wikipedia.org/wiki/Markdown), first clone this repository, then install [pandoc](https://pandoc.org/), change to the [presentation](/presentation) subdirectory, and run:

`pandoc -s --webtex -i -t slidy iteration.md -o iteration.html`

And in the [exercises](/exercises) subdirectory, run:

`pandoc -s --webtex -i -t slidy exercises.md -o exercises.html`

You can then open _iteration.html_ in your favourite browser.

## License

GNU General Public License v3.0

See [COPYING](/COPYING.txt) to see the full text.
