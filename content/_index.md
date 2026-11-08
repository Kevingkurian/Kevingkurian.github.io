---
# Leave the homepage title empty to use the site title
title: ''
summary: ''
date: 2025-11-08
type: landing

sections:
  - block: resume-biography-3
    content:
      # Choose a user profile to display (a folder name within `content/authors/`)
      username: me
      # Short first-person research statement shown next to the profile
      text: |-
        I am a Computer Science PhD student at the University of Florida, advised by Dr. Christan Grant in the UF Data Studio. I study multi-agent LLM systems and how to interpret what happens inside them: how LLM agents reason about one another in strategic settings, how collaboration and feedback loops shape their behavior, and how we can explain and audit the decisions these systems make. My recent work includes evaluating LLM social cognition through multi-agent strategic games, measuring context-switching costs in hybrid LLM-algorithm systems, and building interactive diagnostics for fairness auditing. I have also spent summers on applied AI research at Pacific Northwest National Laboratory, Oak Ridge National Laboratory, and the Software Engineering Institute at Carnegie Mellon University. I am always happy to talk about collaborations in multi-agent systems and LLM interpretability.
      # Show a call-to-action button under your biography? (optional)
      button:
        text: Download CV
        url: uploads/resume.pdf
      headings:
        about: 'My Research'
        education: ''
        interests: ''
    design:
      # Use the new Gradient Mesh which automatically adapts to the selected theme colors
      background:
        gradient_mesh:
          enable: true

      # Name heading sizing to accommodate long or short names
      name:
        size: md # Options: xs, sm, md, lg (default), xl

      # Avatar customization
      avatar:
        size: medium # Options: small (150px), medium (200px, default), large (320px), xl (400px), xxl (500px)
        shape: circle # Options: circle (default), square, rounded
  - block: collection
    id: papers
    content:
      title: Publications
      # Show all publications (0 = no limit)
      count: 0
      filters:
        folders:
          - publications
      # Order by the `weight` set in each publication: first-author papers first, then by date
      sort_by: Weight
      order: asc
    design:
      view: citation
---
