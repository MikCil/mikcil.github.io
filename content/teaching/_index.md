---
title: Teaching
summary: My courses
type: landing

# Template demo section: not published (keeps placeholder pages out of Google)
build:
  render: never
  list: never
  publishResources: false

cascade:
  - _target:
      kind: page
    params:
      show_breadcrumb: true
    build:
      render: never
      list: never
      publishResources: false

sections:
  - block: collection
    id: teaching
    content:
      title: Teaching
      filters:
        folders:
          - teaching
    design:
      view: article-grid
      columns: 2
---
