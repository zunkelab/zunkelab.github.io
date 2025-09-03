---
title: Home
date: 2025-09-01
type: landing

sections:
  - block: slider
    content:
      slides:
        - title: "🔬 Welcome to the Zunke Lab"
          content: "We study the molecular mechanisms of neurodegeneration with a focus on Parkinson’s disease."
          align: center
          background:
            image:
              filename: Lab+robin+johannes.jpg
              filters:
                brightness: 0.6
            position: center
            color: '#444'

        - title: "Our Research"
          content: "Lysosomal biology • Alpha-synuclein • Biomarkers • Astrocytes"
          align: left
          background:
            image:
              filename: Lab+fanny.jpg
              filters:
                brightness: 0.7
            position: center
            color: '#333'
          link:
            icon: microscope
            icon_pack: fas
            text: "Explore Projects"
            url: "/research/"

        - title: "Meet the Team 👥"
          content: "Get to know the scientists behind the discoveries."
          align: right
          background:
            image:
              filename: lab-funny.jpg
              filters:
                brightness: 0.6
            position: center
            color: '#222'
          link:
            icon: users
            icon_pack: fas
            text: "Our People"
            url: people/
    design:
      is_fullscreen: true
      loop: true
      interval: 4000
---
