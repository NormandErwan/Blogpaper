---
author: Erwan Normand
title: Style Guide
subtitle: Demonstration of this theme on an example post page
date: 2020-01-04
tags:
  - markdown
  - css
  - html
  - showcase
  - text
  - shortcodes
categories:
  - themes
  - syntax
series:
  - Themes Guide
banner:
  caption: Alexey Topolyanskiy
  href: https://unsplash.com/photos/-oWyJoSqBRM
---

The Style Guide provides you with a set of standards for the writing and design of theme posts and pages, either for
general use or for a specific publication, organization, or field.
<!--more-->

See these Markdown quick reference for more details on the Markdown syntax: <https://www.markdownguide.org/cheat-sheet>
or <https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet>.

## Images

This theme supports regular image, wide images and full-width images, all with or without the caption.

{{< figure src="1016-730x487.jpg" caption="A regular image with caption. [Philippe Wuyts](https://unsplash.com/photos/_h7aBovKia4)." >}}

{{< figure src="116-1050x600.jpg" caption="A wide image with caption. [Anton Sulsky](https://unsplash.com/photos/YcfCXxo7rpc)." class="wide-width" >}}

{{< figure src="banner.jpg" caption="A full-width image with caption. [Alexey Topolyanskiy](https://unsplash.com/photos/-oWyJoSqBRM)." class="full-width" >}}

## This is an H2

Lorem ipsum dolor sit amet, consectetur adipiscing elit. Aliquam rhoncus enim ut tortor feugiat pulvinar. Nam ac mauris
gravida, porttitor augue ut, ultrices quam. Sed at mollis arcu, ac egestas tellus.

### This is an H3

Mauris a tortor et felis rutrum dignissim. Morbi vel est odio. Suspendisse et ipsum in elit laoreet eleifend vel ac
sapien. Etiam dolor elit, dictum eleifend velit a, pulvinar imperdiet ex.

#### This is an H4

Phasellus sollicitudin, metus nec interdum pellentesque, nunc est ultricies nisl, eu egestas ipsum magna eu purus.
Fusce interdum ultricies ante eu ullamcorper.

## Quoting

> “Creativity is allowing yourself to make mistakes. Design is knowing which ones to keep.”
> — <cite>Scott Adams</cite>

## Code Blocks

Code blocks, highlighted with Hugo's internal highlight shortcode. Read more how to use it on
[Syntax Highlighting page on Hugo docs](https://gohugo.io/content-management/syntax-highlighting/).

{{< highlight html >}}
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Example HTML5 Document</title>
</head>
<body>
  <p>Test</p>
</body>
</html>
{{< /highlight >}}

{{< highlight js >}}
// Simple map
var map;
function initMap() {
  map = new google.maps.Map(document.getElementById('map'), {
    center: {lat: -34.397, lng: 150.644},
    zoom: 8
  });
}
{{< /highlight >}}

{{< highlight css >}}
@import url(http://fonts.googleapis.com/css?family=Arvo);

/* Styles */

body {
  font: 100%/1.5 Questrial, sans-serif;
  tab-size: 4;
  hyphens: auto;
}
{{< /highlight >}}

## Lists

### Ordered List

1. First item
2. Second item
3. Third item

### Unordered List

- List item
- Another item
- And another item

### Nested list

- Item
    1. First Sub-item
    2. Second Sub-item

1. Second list
    - First Sub-item
    - Second Sub-item

## Footnotes

The quick brown fox[^1] jumped over the lazy dog[^2].

[^1]: Foxes are red

[^2]: Dogs are usually not red

Footnotes are a great way to add additional contextual details when appropriate. Hugo will automatically add footnote
content to the very end of your post.

## Tables

| Tables        | Are           | Cool  |
| ------------- |:-------------:| -----:|
| col 3 is      | right-aligned | $1600 |
| col 2 is      | centered      |   $12 |
| zebra stripes | are neat      |    $1 |

Tables are aligned to left by default and take the full width of the page.
Any [column can be aligned](https://www.markdownguide.org/extended-syntax/#alignment) left, center or right.
They can contain any markdown content.

Markdown | Less | Pretty
--- | --- | ---
*Still* | `renders` | **nicely**
1 | 2 | 3

Table examples are from here: <https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet#tables>.

## Videos

{{< vimeo_simple 137643135 >}}

[This Mountain](https://vimeo.com/137643135) from [Evan Mann / OWP Denver](https://vimeo.com/evanmann) on
[Vimeo](https://vimeo.com).

{{< youtube ZJthWmvUzzc >}}

[For the Love of Type](https://www.youtube.com/watch?v=ZJthWmvUzzc) from
[ChingPaul](https://www.youtube.com/channel/UCSMMVkOa__BoWirO8tgxIYw) on
[YouTube](https://www.youtube.com).