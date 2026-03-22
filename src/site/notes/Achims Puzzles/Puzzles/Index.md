---
{"dg-publish":true,"dg-path":"Index.md","permalink":"/index/","noteIcon":"","created":"2026-03-22T17:55:47.336+01:00","dg-note-properties":{}}
---



```base
filters:
  and:
    - file.tags.contains("puzzle")
    - file.folder == "Achims Puzzles/Puzzles"
formulas:
  image: image(file.embeds[0])
views:
  - type: table
    name: Table
    filters:
      and:
        - Ownership != "Me"
    order:
      - file.name
      - formula.image
      - Artist
      - banner
      - Brand
      - Date Aquired
      - Days
      - Difficulty Level
      - End
      - icon
      - Missing Pieces
      - Obtained From
      - Ownership
      - Pieces
      - Quality
      - rating
      - Start
      - Status
      - tags
      - Wo
      - Wohin?
  - type: cards
    name: View
    order:
      - file.name
      - Pieces
    image: formula.image
    imageFit: ""
    cardSize: 260
    imageAspectRatio: 0.45

```
