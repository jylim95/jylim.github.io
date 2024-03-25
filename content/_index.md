---
# Leave the homepage title empty to use the site title
title: ''
date: 2024-03-24
type: landing

sections:
  - block: about.biography
    id: about
    content:
      title: Biography
      # Choose a user profile to display (a folder name within `content/authors/`)
      username: admin
  - block: portfolio
    id: posts
    content:
      title: Recent Posts
      subtitle: ''
      text: ''
      # Choose how many pages you would like to display (0 = all pages)
      count: 3
      # Filter on criteria
      filters:
        folders:
          - post
      default_button_index: 0
      buttons:
        - name: All
          tag: '*'
        - name: Talks
          tag: talks
        - name: Work
          tag: work
        - name: Personal
          tag: personal
    design:
      # Choose a layout view
      view: showcase
      columns: '1'
      flip_alt_rows: true
  - block: collection
    id: featured
    content:
      title: Featured Publications
      count: 3
      filters:
        folders:
          - publication
        featured_only: true
    design:
      columns: '2'
      view: card
  - block: collection
    content:
      title: Recent Publications
      text: |-
        {{% callout note %}}
        You can filter all publications by clicking [here](./publication/).
        {{% /callout %}}
      filters:
        folders:
          - publication
        exclude_featured: true
    design:
      columns: '2'
      view: citation
  - block: markdown
    content:
      title: Through My Eyes 
      subtitle: ''
      text: |-
        {{< gallery album="demo" >}}
    design:
      columns: '1'
  - block: contact
    id: contact-me
    content:
      title: Contact
      email: juinyau95@gmail.com
      address:
        city: Seoul
        country: South Korea
      # Choose a map provider in `params.yaml` to show a map from these coordinates
      coordinates:
        latitude: '37.5894'
        longitude: '127.0325'  
      # Automatically link email and phone or display as text?
      autolink: true
      # Email form provider
    design:
      columns: '2'
---
