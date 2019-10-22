# Selection

> Multiple selections, inspired by [Kakoune].

[![Selection demo](https://img.youtube.com/vi_webp/KIsOSIQXAVU/maxresdefault.webp)](https://youtu.be/KIsOSIQXAVU)

## Usage

On <https://kakoune.org>:

``` javascript
const selections = new SelectionList

// Getting Started
const getStarted = document.querySelector('a[href*="getting-started"]')

selections.add(getStarted) // Select “Getting Started”
selections.parent(2) // Select the navigation section
selections.select('a') // Select all links
selections.focus(getStarted) // Select “Getting Started”
selections.next(2) // Select “Issue Tracker”
selections.children() // Select all of the child elements
selections.previous() // Select the bug icon
selections.remove() // Remove the element from the selections
```

More examples at [Krabby].

## References

- [Create a keyboard interface to the web]

[Kakoune]: https://kakoune.org
[Krabby]: https://github.com/alexherbo2/krabby
[Create a keyboard interface to the web]: https://alexherbo2.github.io/blog/chrome/create-a-keyboard-interface-to-the-web/
