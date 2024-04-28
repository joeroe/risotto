# 🍚 risotto

risotto is a minimalist, responsive [hugo](https://gohugo.io) theme inspired by terminal ricing aesthetics.

[![Hugo Themes](https://img.shields.io/badge/Hugo_Themes-risotto-blue?logo=hugo)](https://themes.gohugo.io/themes/risotto/)
[![Version](https://img.shields.io/badge/semver-v0.4.0-blue)](https://semver.org)
![hugo build status](https://github.com/joeroe/risotto/actions/workflows/hugo-build-exampleSite.yml/badge.svg)
[![W3C Validation](https://img.shields.io/w3c-validation/html?targetUrl=https%3A%2F%2Frisotto.joeroe.io)](https://validator.nu/?doc=https%3A%2F%2Frisotto.joeroe.io)
![Code size](https://img.shields.io/github/languages/code-size/joeroe/risotto)

![Screenshot of the risotto theme](https://raw.githubusercontent.com/joeroe/risotto/master/images/screenshot.png)

## Features

* Plain, semantic HTML with no Javascript
* Plain CSS – no frameworks, no preprocessors, just simple and easy-to-customise stylesheets
* Uses [CSS Grid](https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_grid_layout) for native responsive behaviour without arbitrary breakpoints
* Comes with [16 built-in colour schemes](#colour-schemes) based on popular terminal themes plus the ability to use custom themes using the [base16 system](https://github.com/monicfenga/base16-styles)

## Install

The easiest way to install the theme is to [download the latest release](https://github.com/joeroe/risotto/releases) and extract it to your project's `themes/` directory.
You can also clone this repository into your site's `themes` directory and checkout the latest release:

```shell
git clone https://github.com/joeroe/risotto themes/risotto && cd themes/risotto
git checkout $(git tag -l | grep '^v[0-9.]*$' | sort -V | tail -n 1)
```

Note that this will not work if your site is itself a git repository.
In that case, you can add the theme as a [git submodule](https://git-scm.com/book/en/v2/Git-Tools-Submodules), but this is not recommended due to the difficulty of tracking a specific release.

## Update

If you installed the theme using `git clone`, pull the repository to get the latest version:

```shell
cd themes/risotto
git pull
```

Otherwise, simply [download the latest release](https://github.com/joeroe/risotto/releases) and extract it to your project's `themes/` directory, replacing the old version.

## Configure

To use the theme, add `theme = 'risotto'` to your site's `hugo.toml`, or `theme: risotto` to your `hugo.yaml`.

See `exampleSite/config.toml` for the theme-specific parameters you need to add to your site's `hugo.toml` or `hugo.yaml` to configure the theme.

### Colour schemes

risotto uses the [base16 framework](https://github.com/chriskempson/base16) to define colour schemes that can be used with the `theme.palette` parameter.
A selection of 16 palettes (10 dark, 6 light) are bundled with the theme: `apprentice`, `base16-dark`, `base16-light`, `dracula`, `gruvbox-dark`, `gruvbox-light`, `material`, `papercolor-dark`, `papercolor-light`, `solarized-dark`, `solarized-light`, `tender`, `tokyo-night-dark`, `tokyo-night-light`, `windows-95` and `windows-95-light`.
The default is `base16-dark`.

<!-- TODO: add screenshots of default themes -->

The easiest way to use other base16 styles is to place .css file from https://github.com/monicfenga/base16-styles/tree/master/css-variables and place it in your `static/css/palettes` directory.

Or to define a wholly custom theme, you will need to define the following CSS variables for the following base16 colours (see [base16-dark.css](blob/main/static/css/palettes/base16-dark.css) for an example):

| Base | Default colour                             | Used for            | Examples                             |
| ---- | ------------------------------------------ | ------------------- | ------------------------------------ |
| 00   | <span class="base00">Dark</span>           | Background          | Page background                      |
| 01   | <span class="base01">│</span>              | Alt. background     | Content background                   |
| 02   | <span class="base02">│</span>              | In-text backgrounds | `<pre>`, `<code>`, `<kbd>`, `<samp>` |
| 03   | <span class="base03">│</span>              | Muted text          | `:before` & `:marker` symbols        |
| 04   | <span class="base04">│</span>              | Alt. foreground     | Aside text                           |
| 05   | <span class="base05">│</span>              | Foreground          | Content text                         |
| 06   | <span class="base06">│</span>              |                     |                                      |
| 07   | <span class="base07">Light</span>          |                     |                                      |
| 08   | <span class="base08">Red</span>            |                     |                                      |
| 09   | <span class="base09">Orange</span>         |                     |                                      |
| 0A   | <span class="base0A">Yellow</span>         | Highlights          | Selected text, `<mark>`              |
| 0B   | <span class="base0B">Green</span>          | Primary accent      | Logo                                 |
| 0C   | <span class="base0C">Cyan</span>           | Active links        | `a:active`, `a:hover`                |
| 0D   | <span class="base0D">Blue</span>           | Links               | `a:link`, `a:visited`                |
| 0E   | <span class="base0E">Magenta</span>        |                     |                                      |
| 0F   | <span class="base0F">Brown</span>          |                     |                                      |

For light mode palettes, the sequence of 00–07 should be reversed (light to dark, not dark to light).
Note that not all colours are currently used in the theme.

You you use these colours directly in content using the convenience classes `.baseXX` and `.bg-baseXX`.
For example:

```html
<span class="base0A">Yellow text</span>
<mark class="bg-base0D">Text highlighted in green</mark>
```

## Favicon

risotto will automatically use favicons placed in the `static/` directory.
The following files will be detected and included in your site's `<head>` section:

* `favicon.ico`
* `favicon-16x16.png`
* `favicon-32x32.png`
* `apple-touch-icon.png`
* `site.webmanifest`

You can generate these from an image or emoji using [favicon.io](https://favicon.io/) or a similar service.
They must be placed directly under your site's `static/` directory, i.e. not in in a subdirectory or `themes/risotto/static/`.

## Acknowledgements

The 'cooked rice' emoji used as a favicon for the example site was created by the [Twemoji project](https://twemoji.twitter.com/) and is licensed under [CC-BY 4.0](https://creativecommons.org/licenses/by/4.0/).
