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

## Configure

To use the theme, add `theme = risotto` to your site's `config.toml` or `config.yaml`.

See `exampleSite/config.toml` for the theme-specific parameters you need to add to your site's `config.toml` or `config.yaml` to configure the theme.

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

