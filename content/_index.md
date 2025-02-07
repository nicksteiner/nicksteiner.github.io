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
    content:
      # Choose a user profile to display (a folder name within `content/authors/`)
      username: admin
      text: ""
      # Show a call-to-action button under your biography? (optional)
      button:
        text: Download CV
        url: uploads/cv.pdf
    design:
      css_class: dark
      background:
        color: white
        image:
          # Add your image background to `assets/media/`.
          filename: background1.jpg
          filters:
            brightness: 0.3  # Darken the image slightly
            contrast: 1.2  # Increase contrast
            blur: 2  # Optional soft blur for better text readability          
          size: cover
          position: center
          parallax: false
  - block: markdown
    content:
      title: '📚 My Research'
      subtitle: ''
      text: |-
        I am a Research Assistant Professor in the Department of Earth and Atmospheric Sciences at City College of New York. My research focuses on remote sensing, surface hydrology, and environmental science, with applications in wetland monitoring, carbon cycle dynamics, and geospatial intelligence.

        I work with NASA missions such as NISAR and ECOSTRESS, developing methods to improve satellite-based observations of surface water dynamics, soil moisture, and vegetation structure.

        Please reach out to collaborate! 🚀  
    design:
      columns: '1'
  - block: collection
    id: papers
    content:
      title: Featured Publications
      filters:
        folders:
          - publication
        featured_only: true
    design:
      view: article-grid
      columns: 2
  - block: collection
    content:
      title: Recent Publications
      text: ""
      filters:
        folders:
          - publication
        exclude_featured: false
    design:
      view: citation

---
