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
        url: uploads/resume.pdf
    design:
      css_class: dark
      background:
        color: black
        image:
          # Add your image background to `assets/media/`.
          filename: stacked-peaks.svg
          filters:
            brightness: 1.0
          size: cover
          position: center
          parallax: false
  - block: markdown
    content:
      title: 'My Research'
      subtitle: ''
      text: |-
        My research focuses on Multimodal Visual Language Foundation Models (VLMs) for image, video, 3D, and 4D generation and perception.

        I am the first author of 3D-CoMPaT (ECCV Oral) and 3D-CoMPaT++ (TPAMI 2025, accepted), and I led the NeurIPS paper PointNeXt (1,000+ citations). I have served as a core organizer of a CVPR workshop and as a program chair and reviewer for leading AI venues such as TPAMI, IJCV, CVPR, ICCV, AAAI, TCSVT, and NeurIPS.

        I previously interned at Amazon Science (Prime Video, Seattle) and Sony AI (Tokyo), working on VLMs with 2D/3D perception reasoning and music-driven diffusion models for synchronized human dance generation.

        Feel free to reach out for collaboration.
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
  - block: resume-experience
    id: experience
    content:
      username: admin
    design:
      date_format: 'January 2006'
      is_education_first: false
---
