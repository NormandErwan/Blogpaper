# Blogpaper

> A graphical newspaper like blog theme for Hugo.

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

4. Configure on your `config.yml`:

    ```yml
    theme: blogpaper
    title: # Your site title
    author:
      name: # Your name
    copyright: # Optional, will be displayed on site's footer, if this line is removed an default copyright will be generated
    languageCode: en # The language code of your site, by default "en"
    menu:
      main: # The menu to display on top-right of your site, see https://gohugo.io/templates/menu-templates/#site-config-menus
        - name: About
          url: /about
        - name: Posts
          url: /posts
    params:
      datetimeFormat: Mon 2 Jan 2006 # See https://gohugo.io/functions/format for examples
      description: # The description of your site (used on a <meta> tag)
      #mainSections: # List the sections (the subfolders) you want to display on the homepage, "posts" by default
      #- posts
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
