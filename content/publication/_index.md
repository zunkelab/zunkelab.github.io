---
title: Publications
type: landing

sections:
  # Banner mit Bild, weißer Schrift und EINEM mittigen Button
  - block: markdown
    content:
      title: Publications
      text: |
        A selection of our publications is highlighted below.

        <a class="btn btn-primary px-3 py-3" href="https://pubmed.ncbi.nlm.nih.gov/?term=zunke%2C+friederike&sort=date">See all on PubMed</a>
    design:
      columns: '1'
      background:
        image:
          filename: Neuron.png   # liegt idealerweise in assets/media/Neuron.png
          position: center
          size: cover
          text_color_light: true
      spacing:
        padding: ['80px','0','40px','0']
      css_class: text-center fullscreen text-white   # <- erzwingt weiße Schrift

  # Highlights (nur Einträge mit featured: true)
  - block: collection
    content:
      title: Highlights
      count: 10
      filters:
        featured_only: true
        folders: ["publication"]
      order: desc
    design:
      view: citation
      columns: '1'

  # Alle Publikationen (aus content/publication/…)
  - block: collection
    content:
      title: Selected publications
      count: 200
      filters:
        folders: ["publication"]
      order: desc
    design:
      view: citation
      columns: '1'
---
