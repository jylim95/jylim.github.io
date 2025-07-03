---
# Leave the homepage title empty to use the site title
title: ''
date: 2024-12-01
type: landing

sections:
  - block: hero
    content:
      title: |
        Dr. Juin Yau Lim
      image:
        filename: hero-academic.png
      cta:
        label: "**View My Research**"
        url: './publication/'
      cta_alt:
        label: "Download CV"
        url: './uploads/resume.pdf'
      text: |-
        **Sustainable Engineering Expert** 🌱
        
        Passionate about bridging the gap between **research** and **industry** with innovative solutions in:
        
        - 🔬 **Process Systems Engineering**
        - 🤖 **Artificial Intelligence Applications**
        - ♻️ **Renewable Energy & Waste-to-Energy**
        - 🌍 **Environmental Management**
        
        **Ph.D in Applied Environmental Science** | **M.Eng in Chemical Engineering** | **AMIChemE**
        
        Currently advancing sustainable solutions at **Argonne National Laboratory**
    design:
      background:
        gradient_end: '#1976d2'
        gradient_start: '#004ba0'
        text_color_light: true

  - block: about.biography
    id: about
    content:
      title: Biography
      # Choose a user profile to display (a folder name within `content/authors/`)
      username: admin
    design:
      background:
        color: white
        text_color_light: false
      spacing:
        padding: ['20px', '0', '20px', '0']

  - block: stats
    content:
      items:
        - statistic: "40+"
          description: |
            Research Publications
        - statistic: "2"
          description: |
            Advanced Degrees
        - statistic: "5+"
          description: |
            Years Experience
        - statistic: "4"
          description: |
            Languages Spoken
    design:
      background:
        color: '#f8f9fa'
      spacing:
        padding: ['20px', '0', '20px', '0']

  - block: collection
    id: skills
    content:
      title: Core Expertise
      subtitle: Technical Skills & Research Areas
      text: |
        My interdisciplinary expertise spans multiple domains, combining engineering fundamentals with cutting-edge technology.
      items:
        - name: Process Systems Engineering
          description: Advanced process modeling, optimization, and control systems
          icon: cogs
          icon_pack: fas
        - name: Artificial Intelligence
          description: Machine learning applications in environmental and chemical engineering
          icon: brain
          icon_pack: fas
        - name: Renewable Energy
          description: Sustainable energy systems and waste-to-energy technologies
          icon: solar-panel
          icon_pack: fas
        - name: Environmental Management
          description: Environmental impact assessment and sustainable practices
          icon: leaf
          icon_pack: fas
        - name: Data Analytics
          description: Statistical analysis and data-driven decision making
          icon: chart-line
          icon_pack: fas
        - name: Research & Development
          description: Innovation in sustainable engineering solutions
          icon: flask
          icon_pack: fas
    design:
      columns: '3'
      view: showcase
      flip_alt_rows: true

  - block: collection
    id: featured
    content:
      title: Featured Publications
      subtitle: Highlighting impactful research contributions
      count: 3
      filters:
        folders:
          - publication
        featured_only: true
    design:
      columns: '2'
      view: card
      background:
        color: white

  - block: collection
    id: posts
    content:
      title: Latest Insights
      subtitle: Recent thoughts and discoveries
      text: |
        Stay updated with my latest research findings, industry insights, and professional journey.
      # Choose how many pages you would like to display (0 = all pages)
      count: 4
      # Filter on criteria
      filters:
        folders:
          - post
        author: ""
        category: ""
        tag: ""
        exclude_featured: false
        exclude_future: false
        exclude_past: false
        publication_type: ""
      # Choose how many pages you would like to offset by
      offset: 0
      # Page order: descending (desc) or ascending (asc) date.
      order: desc
    design:
      # Choose a layout view
      view: masonry
      columns: '2'
      background:
        color: '#f8f9fa'
      spacing:
        padding: ['20px', '0', '20px', '0']

  - block: collection
    content:
      title: Recent Publications
      text: |-
        {{% callout note %}}
        Explore my complete publication portfolio by clicking [here](./publication/).
        {{% /callout %}}
      count: 6
      filters:
        folders:
          - publication
        exclude_featured: true
    design:
      columns: '2'
      view: citation
      background:
        color: white

  - block: accomplishments
    content:
      title: Professional Achievements
      subtitle: Recognition and milestones
      items:
        - title: Ph.D in Applied Environmental Science and Engineering
          certificate_url: ''
          date_start: '2023-01-01'
          date_end: ''
          description: 'Kyung Hee University (Global) - Specialized in sustainable engineering solutions'
          icon: graduation-cap
          icon_pack: fas
          organization: Kyung Hee University
          organization_url: ''
        - title: M.Eng in Chemical Engineering & Environmental Engineering
          certificate_url: ''
          date_start: '2018-01-01'
          date_end: ''
          description: 'University of Nottingham - Double major in Chemical and Environmental Engineering'
          icon: graduation-cap
          icon_pack: fas
          organization: University of Nottingham
          organization_url: ''
        - title: AMIChemE Membership
          certificate_url: ''
          date_start: '2018-01-01'
          date_end: ''
          description: 'Associate Member of Institution of Chemical Engineers'
          icon: award
          icon_pack: fas
          organization: IChemE
          organization_url: ''
    design:
      columns: '2'
      background:
        color: '#f8f9fa'

  - block: markdown
    content:
      title: Through My Eyes 
      subtitle: 'A glimpse into my professional journey'
      text: |-
        {{< gallery album="demo" >}}
        
        *"Never the smartest mind in class but always the one not afraid of trying new things."*
        
        My journey spans multiple continents and disciplines, from chemical engineering to environmental science, always with a focus on sustainable solutions and innovative approaches.
    design:
      columns: '1'
      background:
        color: white
      spacing:
        padding: ['20px', '0', '20px', '0']
      
  - block: contact
    id: contact-me
    content:
      title: Let's Connect
      subtitle: Ready to collaborate on sustainable engineering solutions?
      text: |
        I'm always interested in discussing new opportunities, research collaborations, or sharing insights about sustainable engineering practices.
        
        **Currently based at:** Argonne National Laboratory, Illinois, USA
      email: limj@anl.gov
      phone: # Add if you want to include phone
      address:
        street: # Add if you want to include street address
        city: Illinois
        region: IL
        postcode: '60439'
        country: United States of America
      # Choose a map provider in `params.yaml` to show a map from these coordinates
      coordinates:
        latitude: '41.7183'
        longitude: '-87.9789'  
      contact_links:
        - icon: linkedin
          icon_pack: fab
          name: Connect on LinkedIn
          link: 'https://www.linkedin.com/in/jylim8/'
        - icon: google-scholar
          icon_pack: ai
          name: Google Scholar
          link: 'https://scholar.google.com/citations?user=6vKIwTgAAAAJ&hl=en'
        - icon: orcid
          icon_pack: ai
          name: ORCID
          link: 'https://orcid.org/0000-0002-2691-4439'
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
      background:
        color: '#1976d2'
        text_color_light: true
---
