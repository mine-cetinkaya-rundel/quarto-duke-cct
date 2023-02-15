# quarto-duke-cct

Hello, Quarto: A World of Possibilities (for Reproducible Publishing) for Duke CCT (2023-02-15)

## Setup notes

- R 4.2.2 (2022-10-31) -- "Innocent and Trusting"
- RStudio 2022.12.0+353 "Elsbeth Geranium"
- Quarto 1.2.335
- Packages: tidyverse, palmerpenguins, gt

## Demo

### Documents

- Create a simple Quarto document called `index.qmd` and edit it using the RStudio Visual Editor with sections Data, Species, and Penguins.
- Add code chunk options:
  - `echo: false` in `execute` in the YAML
  - `code-fold`
  - `fig-alt`
  - teaching tip: `echo: fenced`
- Add a figure and a table and cross reference them
- Add a citation

### Slides

- Change `format: revealjs`
- Add section headings: First level headings Introduction and Analysis, under Analysis a second level heading called Modeling
- Add columns to slides
- Reveal code with `echo: true`
  - teaching-tip: `code-line-numbers`
- Change `output-location` of figure

### Websites

- Add another document `about.qmd`
- Add `quarto.yml` 

```
project:
  type: website

website:
  title: "Hello Quarto - Duke CCT"
  navbar:
    left:
      - index.qmd
      - about.qmd
```

- Render and then `publish quarto`