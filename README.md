# Boolean Iteration

A [presentation](/presentation/iteration.md) on _loops and iteration_ for [Boolean](https://boolean.co.uk/). Included are some [exercises](/exercises/exercises.md), too.

## Install

To recreate the html slideshows from the source [Markdown](https://en.wikipedia.org/wiki/Markdown), first clone this repository, then install [pandoc](https://pandoc.org/), change to the [presentation](/presentation) subdirectory, and run:

`pandoc -s --webtex -i -t slidy iteration.md -o iteration.html`

And in the [exercises](/exercises) subdirectory, run:

`pandoc -s --webtex -i -t slidy exercises.md -o exercises.html`

You can then open _iteration.html_ and exercises.html in your favourite browser.

## License

GNU General Public License v3.0

See [COPYING](/COPYING.txt) to see the full text.
