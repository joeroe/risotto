# risotto

risotto is a minimalist, responsive [hugo](https://gohugo.io) theme inspired by terminal ricing aesthetics.

![Screenshot of the risotto theme](https://raw.githubusercontent.com/joeroe/risotto/master/images/screenshot.png)

## Install

The easiest way to install the theme is to clone this repository into your site's `themes` directory:

```shell
git clone https://github.com/joeroe/risotto themes/risotto
```

If your site is already a git repository, you can add the theme as a submodule instead:

```shell
git submodule add https://github.com/joeroe/risotto.git themes/risotto
```

## Update

If you installed the theme using `git clone`, pull the repository to get the latest version:

```shell
cd themes/risotto
git pull
```

Or, if you added it as a git submodule:

```shell
git submodule update --remote
```

## Configure

To use the theme, add `theme = risotto` to your site's `config.toml` or `config.yaml`.

See `exampleSite/config.toml` for the theme-specific parameters you need to add to your site's `config.toml` or `config.yaml` to configure the theme.

### Colour palettes

Colour palettes for the theme are defined using the [base16 system](https://github.com/chriskempson/base16):

| Base | Default colour | Used for | Examples |
| ---- | -------------- | -------- | -------- |
| 00   | Dark           | Background | Page background          |
| 01   | │              | Alt. background | Content background          |
| 02   | │              | In-text backgrounds | `<pre>`, `<code>`, `<kbd>`, `<samp>` |
| 03   | │              | Muted text | `:before` & `:marker` symbols |
| 04   | │              | Alt. foreground | Aside text          |
| 05   | │              | Foreground         | Content text         |
| 06   | │              |          |          |
| 07   | Light          |          |          |
| 08   | Red            |          |          |
| 09   | Orange         |          |          |
| 0A   | Yellow         | Highlights | Selected text, `<mark>` |
| 0B   | Green          | Primary accent | Logo          |
| 0C   | Cyan           | Active links | `a:active`, `a:hover`         |
| 0D   | Blue           | Links    | `a:link`, `a:visited`         |
| 0E   | Magenta        |          |          |
| 0F   | Brown          |          |          |

For light mode palettes, the sequence of 00–07 should be reversed (light to dark, not dark to light).
