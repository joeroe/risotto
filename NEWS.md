# risotto (development version)

* **Breaking change** – new framework for colour palettes:
  * Palettes are defined using CSS variables following the [base16](https://github.com/chriskempson/base16) system
  * Added 2 new palettes: `base16-dark` and `base16-light`
  * The default palette is `base16-dark`
  * The `mode` parameter is no longer needed
  * If you were using one of the old named palettes (`gruvbox-dark` or `gruvbox-light`), the change will be seamless
  * If you were using a custom palette, you will need to redefine it using the new framework
* Added a table of contents (thanks @dashv, #47)
* Added multilanguage support with a language switcher (thanks @bedefaced)
* Added a changelog

# risotto 0.1.0

First named release, including:

* `gruvbox-dark` and `gruvbox-light` colour palettes
* FontAwesome6 and Academicons icon sets
