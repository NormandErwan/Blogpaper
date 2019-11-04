# Blogpaper

> A newspaper like blog theme for Hugo.

## Install

Get the theme:

```bash
git submodule add https://github.com/NormandErwan/blogpaper themes/blogpaper
cd themes/blogpaper
yarn install
```

Preview the example site:

```bash
hugo server -c themes/blogpaper/exampleSite/ -s themes/blogpaper/
```

Change your `config.toml`:

```toml
theme = "blogpaper"
```

## Upgrade

Execute:

```bash
git submodule update --remote themes/blogpaper
yarn install
```

## License

The MIT License (MIT). Copyright (c) 2019 Erwan Normand <normand.erwan@protonmail.com>.

See the [LICENSE](LICENSE) file for details.
