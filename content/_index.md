---
# Leave the homepage title empty to use the site title
title: ''
date: 2022-10-24
type: landing

design:
  # Default section spacing
  spacing: '6rem'

sections:
  - block: resume-biography-3
    content:
      # Choose a user profile to display (a folder name within `content/authors/`)
      username: admin
      # ✅ Use a multiline block for rich text with links
      text: |
        I am a researcher in recommender systems and trustworthy AI. I completed my PhD in Computer Science at the University of Amsterdam, advised by
        <strong><a href="https://scholar.google.com/citations?user=AVDkgFIAAAAJ" target="_blank" rel="noopener">Prof. dr. Maarten de Rijke</a></strong>.
        Before that, I worked with
        <strong><a href="https://scholar.google.com/citations?user=X45Go24AAAAJ" target="_blank" rel="noopener">Prof. dr. Xiangnan He</a></strong>
        and
        <strong><a href="https://scholar.google.com/citations?user=HdhaQB0AAAAJ" target="_blank" rel="noopener">Prof. dr. Xiang Wang</a></strong>.

        My work focuses on generative recommendation, LLM agents for recommendation, and the safety and robustness of recommender systems, especially in sensitive domains such as news recommendation and personalized content delivery, where user trust and experience are critical.
      # Show a call-to-action button under your biography (optional)
      button:
        text: Download CV
        url: uploads/CV_YZhao.pdf
      headings:
        about: ''
        education: ''
        interests: ''
    design:
      # Apply a gradient background
      css_class: hbx-bg-gradient
      # Avatar customization
      avatar:
        size: medium # small / medium / large / xl / xxl
        shape: circle # circle / square / rounded

  - block: collection
    id: papers
    content:
      title: Featured Publications
      filters:
        folders:
          - publications
        featured_only: true
    design:
      view: article-grid
      columns: 2

  - block: collection
    id: recent-pubs
    content:
      title: Recent Publications
      text: ''
      filters:
        folders:
          - publications
        exclude_featured: false
    design:
      view: citation
---
