---
# Leave the homepage title empty to use the site title
title:
date: 2022-10-24
type: landing

sections:
  - block: about.biography
    id: about
    content:
      title: Biography
      # Choose a user profile to display (a folder name within `content/authors/`)
      username: admin
  - block: collection
    id: book
    content:
      title: Book
      filters:
        folders:
          - publication
        featured_only: true
    design:
      columns: '2'
      view: card
  - block: collection
    id: articles
    content:
      title: Selected Articles
      text: |-
      filters:
        folders:
          - publication
        exclude_featured: true
    design:
      columns: '2'
      view: citation
  - block: contact
    id: contact
    content:
      title: Contact
      text: |-
      # Contact (add or remove contact options as necessary)
      email: thomas.matthew.vozar@uni-hamburg.de
      address:
        street: Phil-Turm, Von-Melle-Park 6, 20146 Hamburg, Germany
        city:
        region:
        postcode: ''
        country:
        country_code: DE
      office_hours:
        - 'By appointment'
      # Automatically link email and phone or display as text?
      autolink: true
      # Email form provider
      form:
        provider: netlify
        formspree:
          id:
        netlify:
          # Enable CAPTCHA challenge to reduce spam?
          captcha: false
    design:
      columns: '2'
---
