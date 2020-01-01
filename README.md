# Blogpaper

> A graphical newspaper like blog theme for Hugo.

[![Quality Gate Status](https://sonarcloud.io/api/project_badges/measure?project=NormandErwan_blogpaper&metric=alert_status)](https://sonarcloud.io/dashboard?id=NormandErwan_blogpaper)

![Example of a homepage](images/screenshot.jpg)

![Example of a post page](images/post-page.jpg)

This theme is inspired by [Start Bootstrap - Clean Blog](https://github.com/BlackrockDigital/startbootstrap-clean-blog),
Jekyll's [Olania](https://olania-jekyll.netlify.com/) and Jekill's [Curious](https://curious-jekyll.netlify.com/).

## Install

1. Make sure you're using the [Hugo extended](https://gohugo.io/getting-started/installing/) version.
2. Get the theme:

    ```bash
    git submodule add https://github.com/NormandErwan/Blogpaper themes/Blogpaper
    ```

3. Edit your `config.yml`:

    ```yml
    theme: Blogpaper
    ```

4. Generate your site!

    ```bash
    hugo server -D
    ```

You should now a have a working blog, but with a flat grey background instead of banner images on top your pages. See
the next section to configure your blog and add banner images on your pages.

|                           After intall homepage                           |                           After intall post page                            |
|:-------------------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| ![Example of a homepage after install](images/after-install-homepage.jpg) | ![Example of a post page after install](images/after-install-post-page.jpg) |

## Configure

1. Edit your `config.yml`:

    ```yml
    theme: Blogpaper
    title: # Your site title
    author:
      name: # Your name
    baseURL: # Hostname (and path) to the root, e.g. https://bep.is/ (Blogpaper uses relative URLs)
    copyright: # Optional, will be displayed on site's footer, if this line is removed an default copyright will be generated
    languageCode: en # The language code of your site, by default "en"
    menu:
      main: # Optional, the menu to display on top-right of your site, see https://gohugo.io/templates/menu-templates/#site-config-menus
        - name: About
          url: /about
    params:
      description: # The description of your site (used on a <meta> tag)
      mainSections: # Optional, list the sections (the subfolders) you want to display on the homepage, "posts" by default
        - posts
    ```

    See <https://gohugo.io/getting-started/configuration/> for more configuration settings (such as `datetimeFormat`,
    `paginate` or `summaryLength`).

2. Add banner images on your pages, you can either:
    - Add a `banner.jpg` image next to a `index.md` or `_index.md` page.
    - Add a `<page-filename>.jpg` image next to a `<page-filename>.md` page.
    - Add no image to use the banner of the parent page.
    - Use a custom image by adding to the front matter of the page:

        ```yml
        banner:
          src: <banner-filename>.jpg # Optional, the filename of the banner, by default <page-filename>.md or banner.jpg
        ```

    - Set no banner by adding to the front matter of the page:

        ```yml
        banner: false
        ```

3. You can add a caption and link on a banner, add to the
[front matter](https://gohugo.io/content-management/front-matter/) of the page:

    ```yml
    banner:
      src: <banner-filename>.jpg # Optional, the filename of the banner, by default <page-filename>.md or banner.jpg
      caption: # Optional, the caption of the banner
      href: # Optional, a link on the caption
    ```

See for example the Blogpaper's [example site](https://github.com/NormandErwan/BlogpaperExampleSite):

```bash
.
└── content
    ├── posts
    |   ├── rich-content
    |   |   ├── banner.jpg
    |   |   └── index.md # Use banner.jpg
    |   ├── _index.md # No banner.jpg, use the parent banner: ../banner.jpg
    |   └── emoji-support.md # Use emoji-support.jpg
    |   ├── emoji-support.jpg
    |   └── ...
    ├── _index.md # Use banner.jpg
    ├── about.md # Use about.jpg
    ├── about.jpg
    └── banner.jpg
```

You can download free images on sites like [Lorem Picsum](https://picsum.photos/) or
[other](https://alternativeto.net/software/unsplash/).

## Troubleshooting / FAQ

- I can't generate the site.
  - Problem: I have the error: `Problem: Building sites … ERROR Transformation failed: TOCSS: failed to transform "blogpaper.scss" (text/x-scss)`.
  - Solution: [Reinstall Hugo](https://gohugo.io/getting-started/installing/), the *extended* version not the standard one.

## Upgrade

Execute:

```bash
git submodule update --remote themes/Blogpaper
```

## License

The MIT License (MIT). Copyright (c) 2019 Erwan Normand <normand.erwan@protonmail.com>.

See the [LICENSE](LICENSE) file for details.
