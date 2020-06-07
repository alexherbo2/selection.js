# selection.js

selection.js is a JavaScript library to manipulate multiple selections, inspired by [Kakoune].

[Kakoune]: https://kakoune.org

[![selection.js](https://img.youtube.com/vi_webp/KIsOSIQXAVU/maxresdefault.webp)](https://youtube.com/playlist?list=PLdr-HcjEDx_k12ybIzEREKrdQGqj48HTJ "YouTube – selection.js")
[![YouTube Play Button](https://www.iconfinder.com/icons/317714/download/png/16)](https://youtube.com/playlist?list=PLdr-HcjEDx_k12ybIzEREKrdQGqj48HTJ) · [selection.js](https://youtube.com/playlist?list=PLdr-HcjEDx_k12ybIzEREKrdQGqj48HTJ)

## Installation

Add [`selection.js`](src/selection.js) and [`selection.css`](src/selection.css) to your project.

## Usage

Navigate to <https://kakoune.org>:

``` javascript
const selections = new SelectionList

// Getting Started
const getStarted = document.querySelector('a[href*="getting-started"]')

selections.add(getStarted) // Selects “Getting Started”
selections.parent(2) // Selects the navigation section
selections.select('a') // Selects all links
selections.focus(getStarted) // Selects “Getting Started”
selections.next(2) // Selects “Issue Tracker”
selections.children() // Selects all of the child elements
selections.previous() // Selects the bug icon
selections.remove(selections.mainSelection) // Removes the main selection
```

You can find some examples in [Krabby].

[Krabby]: https://krabby.netlify.app

See the [source](src/selection.js) for a complete reference.
