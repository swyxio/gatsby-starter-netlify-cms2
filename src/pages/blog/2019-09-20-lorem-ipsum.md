---
templateKey: blog-post
title: Lorem Ipsum
date: 2019-09-22T02:04:25.762Z
description: Foo bar baz whatever
featuredpost: true
featuredimage: /img/shawn-wang-card-c7351f1039c377d8e3bf5ccf2e574641.png
tags:
  - tech
  - javascript
---


collections:
  - name: "blog"
    label: "Blog"
    folder: "src/pages/blog"
    create: true
    slug: "{{year}}-{{month}}-{{day}}-{{slug}}"
    fields:
      - {label: "Template Key", name: "templateKey", widget: "hidden", default: "blog-post"}
      - {label: "Title", name: "title", widget: "string"}
      - {label: "Publish Date", name: "date", widget: "datetime"}
      - {label: "Description", name: "description", widget: "text"}
      - {label: "Featured Post", name: "featuredpost", widget: "boolean"}
      - {label: "Featured Image", name: "featuredimage", widget: image}
      - {label: "Body", name: "body", widget: "markdown"}
      - {label: "Tags", name: "tags", widget: "list"}

  - name: "pages"
    label: "Pages"
    files:
      - file: "src/pages/index.md"
        label: "Landing Page"
        name: "index"
        fields:
          - {label: "Template Key", name: "templateKey", widget: "hidden", default: "index-page"}
          - {label: Title, name: title, widget: string}
