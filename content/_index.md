---
# Leave the homepage title empty to use the site title
title: ""
date: 2022-10-24
type: landing

design:
  # Default section spacing
  spacing: "6rem"

sections:
  - block: resume-biography-3
    title: Biographie
    content:
      # Choose a user profile to display (a folder name within `content/authors/`)
      username: admin
      text: ""
      # Show a call-to-action button under your biography? (optional)
     # button:
      #  text: Download CV
       # url: uploads/resume.pdf
    design:
      css_class: dark
      background:
        #color: 
        #image:
          # Add your image background to `assets/media/`.
          #filename: stacked-peaks.svg
          #filters:
           # brightness: 1.0
          #size: cover
          #position: center
          #parallax: false
  - block: collection
    id: publications
    content:
      title: Publications
      text: ""
      headless: true
      count: 0
      offset: 0
      filters:
        folders:
          - publication
        featured_only: true
      design:
        view: citation
        columns: 2
  - block: collection
    content:
      title: Autres textes
      text: ""
      filters:
        folders:
          - publication
        exclude_featured: true
    design:
      view: citation
      columns: 2
  - block: collection
    id: talks
    content:
      title: Exposés récents ou  à venir
      filters:
        folders:
          - event
    design:
      view: list
      columns: 2
      flip_alt_rows: true

        
  
---