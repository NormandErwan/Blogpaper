---
title: {{ replace .TranslationBaseName "-" " " | title }}
subtitle: # Optional, will be displayed bellow the title of the page; remove this line to generate an automatic subtitle
date: {{ .Date }}
categories: # Optional, will be displayed above the title of the page
- First category
- Second category
tags: # Optional, will be displayed at the bottom end of the post
- First tag
- Second tag
summary: # Optional, will be diplayed on the homepage; remove this line to generate an automatic summary (see https://gohugo.io/content-management/summaries/)
draft: true
banner:
  #src: {{ .TranslationBaseName }}.jpg # Optional, the filename of the banner, by default {{ .TranslationBaseName }}.jpg
  caption: # Optional, the caption of the banner
  href: # Optional, a link on the caption
---
