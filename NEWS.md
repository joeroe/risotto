# risotto (development version)

* Fix overflow of code blocks with line numbers (#41)
* Add descriptions to sidebar of list pages, where defined in the frontmatter of `_index.md` (#55)

# risotto 0.3.0

* Added support for favicons (#57)

# risotto 0.2.0

* **Breaking change** – new framework for colour palettes:
  * Palettes are defined using CSS variables following the [base16](https://github.com/chriskempson/base16) system
  * Added 14 new palettes: `apprentice`, `base16-dark`, `base16-light`, `dracula`, `material`, `papercolor-dark`, `papercolor-light`, `solarized-dark`, `solarized-light`, `tender`, `tokyo-night-dark`, `tokyo-night-light`, `windows-95` and `windows-95-light`.
  * The default palette is `base16-dark`
  * The `mode` parameter is no longer needed
  * If you were using one of the old named palettes (`gruvbox-dark` or `gruvbox-light`), the change will be seamless.
  * If you were using a custom palette, you will need to redefine it using the new framework. See README for further details.
* Added a table of contents (thanks @dashv, #47)
* Added multilanguage support with a language switcher (thanks @bedefaced)
* Made the site header and nav wrap more efficiently on narrow screens (thanks @m-dev672, #32)
* Added a changelog

# risotto 0.1.0

First named release, including:

* `gruvbox-dark` and `gruvbox-light` colour palettes
* FontAwesome6 and Academicons icon sets
