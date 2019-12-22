# Blogpaper

> A newspaper like blog theme for Hugo.

[![Quality Gate Status](https://sonarcloud.io/api/project_badges/measure?project=NormandErwan_blogpaper&metric=alert_status)](https://sonarcloud.io/dashboard?id=NormandErwan_blogpaper)

This theme is inspired by [Start Bootstrap - Clean Blog](https://github.com/BlackrockDigital/startbootstrap-clean-blog),
Jekyll's [Olania](https://olania-jekyll.netlify.com/) and Jekill's [Curious](https://curious-jekyll.netlify.com/).

## Install

1. Make sure you're using the [Hugo extended](https://gohugo.io/getting-started/installing/) version.
2. Install the package manager [Yarn](https://yarnpkg.com/en/docs/install).
3. Get the theme:

    ```bash
    git submodule add https://github.com/NormandErwan/blogpaper themes/blogpaper
    cd themes/blogpaper
    yarn install
    ```

4. Configure on your `config.toml`:

    ```toml
    theme = "blogpaper"
    title = "" # Your blog title
    copyright = "" # Optional copyright that will be displayed on footer

    [params]
      author = "" # Your name
      datetimeFormat = "Mon 2 Jan 2006" # See https://gohugo.io/functions/format for examples
      description = "" # The description of your site
      mainSections = ["posts", "docs"] # List the sections (the subfolders) you want to display on the homepage
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
