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
    git submodule add https://github.com/NormandErwan/Blogpaper themes/Blogpaper
    yarn -cwd themes/Blogpaper install
    ```

4. Configure on your `config.yml`:

    ```yml
    theme: Blogpaper
    title: # Your site title
    author:
      name: # Your name
    baseURL: # Hostname (and path) to the root, e.g. https://bep.is/ (Blogpaper uses relative URLs)
    copyright: # Optional, will be displayed on site's footer, if this line is removed an default copyright will be generated
    languageCode: en # The language code of your site, by default "en"
    menu:
      main: # The menu to display on top-right of your site, see https://gohugo.io/templates/menu-templates/#site-config-menus
        - name: About
          url: /about
    params:
      description: # The description of your site (used on a <meta> tag)
      mainSections: # List the sections (the subfolders) you want to display on the homepage, "posts" by default
        - posts
    ```

    See <https://gohugo.io/getting-started/configuration/> for more configuration settings (such as `datetimeFormat`,
    `paginate` or `summaryLength`).

5. Add banner images on your pages.
    - You can download images on sites like [Lorem Picsum](https://picsum.photos/) or
    [other](https://alternativeto.net/software/unsplash/).

6. Generate your site!

    ```bash
    hugo server -D
    ```

## Upgrade

Execute:

```bash
git submodule update --remote themes/blogpaper
yarn -cwd themes/Blogpaper install
```

## Troubleshooting / FAQ

- I can't generate the site.
  - Problem: I have the error: `Problem: Building sites … ERROR Transformation failed: TOCSS: failed to transform "blogpaper.scss" (text/x-scss)`.
  - Solution: [Reinstall Hugo](https://gohugo.io/getting-started/installing/), the *extended* version not the standard one.

## License

The MIT License (MIT). Copyright (c) 2019 Erwan Normand <normand.erwan@protonmail.com>.

See the [LICENSE](LICENSE) file for details.
