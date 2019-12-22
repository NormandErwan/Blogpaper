---
title: "{{ replace .TranslationBaseName "-" " " | title }}"
date: {{ .Date }}
categories: # Optional, will be displayed on top of the post's title
- First category
- Second category
tags: # Optional, will be displayed at the bottom end of the post
- First tag
- Second tag
summary: "" # Optional, remove this line for generate an automatic summary; see https://gohugo.io/content-management/summaries/
draft: true
banner: "banner.jpg" # Optional filename to the post's banner, remove this line to use the default value "banner.jpg", set empty to use no banner
resources:
- src: banner.jpg # Optional caption and link to the post's banner
  params:
    caption: "" # The caption
    href: "" # The link
---
