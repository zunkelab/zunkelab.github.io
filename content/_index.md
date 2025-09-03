---
# Leave the homepage title empty to use the site title
title: Zunke Lab
date: 2022-10-24
type: landing

sections:
  - block: hero
    content:
      title: |
        Zunke Lab
        Research Group
      image:
        filename: team.jpg   # <— großes Header-Bild
      text: |
        Welcome to the **Zunke Lab**!
        We investigate Parkinson’s disease and Multiple System Atrophy, with a special focus on how lysosomes contribute to neurodegeneration and how they may be targeted for therapy.
      cta:
        label: "Join us"
        url: "/contact/"     # wenn du auf der gleichen Seite ein Kontakt-Block mit id=contact hast, nutze "#contact"
        icon: ""
      cta_alt:
        label: "Meet the team →"
        url: "/people/"
        icon: ""

  # NEWS & EVENTS nebeneinander (automatisch aus content/post und content/event)
  - block: collection
    content:
      title: News & Events
      subtitle:
      text:
      count: 6
      filters:
        folders: ["post","event"]   # zieht Posts & Events
        exclude_featured: false
      offset: 0
      order: desc
    design:
      view: card
      columns: '2'

  # optionaler Trenner mit Bild (vollbreit)
  - block: markdown
    content:
      title:
      subtitle: ''
      text:
    design:
      columns: '1'
      background:
        image:
          filename: fundings3.png     
          filters:
            brightness: 1
          parallax: false
          position: center
          size: cover
          text_color_light: true
      spacing:
        padding: ['20px', '0', '20px', '0']
      css_class: fullscreen

  # Publikationen (wie gehabt)
  - block: collection
    content:
      title: Latest Prints
      text: ""
      count: 5
      filters:
        folders:
          - publication
        publication_type: 'article'
    design:
      view: citation
      columns: '1'

  # großer Call-to-Action + Link zur Teamseite
  - block: markdown
    content:
      title:
      subtitle:
      text: |
        {{% cta cta_link="./people/" cta_text="Meet the team →" %}}
    design:
      columns: '1'

  # unten: zweites großes Gruppenbild
  - block: markdown
    content:
      title:
      subtitle:
      text:
    design:
      columns: '1'
      background:
        image:
          filename: Kopfklinik.jpg       # <— Gruppenfoto unten
          filters:
            brightness: 1
          parallax: false
          position: center
          size: cover
          text_color_light: true
      spacing:
        padding: ['40px', '0', '40px', '0']
      css_class: fullscreen
---
