---
# Leave the homepage title empty to use the site title
title:
date: 2022-10-24
type: landing

sections:
  - block: hero
    content:
      title: Welcome
      # Reference an image in your `assets/media/` folder
      
    design:
      background:
        text_color_light: true
        # gradient_end: '#1976d2'
        # gradient_start: '#004ba0'
        image:
          filename: DSC_1114.jpg
          size: cover
          position: center
          parallax: true
      spacing:
        padding: ["100px", "0", "300px", "0"]
        
  - block: about.avatar
    id: about
    content:
      # Choose a user profile to display (a folder name within `content/authors/`)
      username: admin
      text:
      # Override your bio text from `authors/admin/_index.md`?
    design: # Doesn't seem to work here
      columns: '2'
      view: showcase
      
      
  - block: portfolio
    id: projects
    content:
      title: Projects
      text: (update coming soon...)
        
      filters:
        folders:
          - project
      # Default filter index (e.g. 0 corresponds to the first `filter_button` instance below).
      default_button_index: 0
    design:
      # Choose how many columns the section has. Valid values: '1' or '2'.
      columns: '2'
      view: showcase
      # For Showcase view, flip alternate rows?
      flip_alt_rows: false
  - block: collection
    id: featured
    content:
      title: Featured Publications
      filters:
        folders:
          - publication
        featured_only: true
    design:
      columns: '2'
      view: card
  - block: collection
    content:
      title: Publications
      text: (update coming soon...)
      count: 0
      filters:
        folders:
          - publication
        exclude_featured: true
    design:
      columns: '2'
      view: citation
---
