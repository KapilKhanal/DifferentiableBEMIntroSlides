---
title: |
  <span style="font-size: .8em;">Differentiable Hydrodynamic Analysis using MarineHydro.jl</span>
subtitle: "**Kapil Khanal$^{1,2}$, Carlos A. Michelén Ströfer$^2$, Matthieu Ancellin$^3$, Maha Haji$^1$**  
<br>  
<small>  
1. Cornell University  
2. Sandia National Laboratories  
3. Eurobios Mews Labs  
</small>"
  
format: revealjs
transition: slide 
footer: '<img src="sealab.png" style="height: 40px;">'
colorlinks: true
auto-stretch: true
css: styles.css
slider: true
slideNumber: true
incremental: true
bibliography: references.bib
title-slide-attributes:
  data-background-image: "cornell.png"
  data-background-size: auto
  data-background-opacity: "0.4"
  data-background-position: "center 80%"
---

### Images
::: {layout-ncol=2}
#### Left Column Text
This is some text that will be on the left side of the slide.

#### Right Column Image
![Surus](sandia.png)
:::



:::: {.columns}

::: {.column width="70%"}
#### Differentiable simulation 
- $$\frac{\partial f(\mathbf{x})}{\partial \mathbf{x}}$$ where $f$ is a simulation model and $x$ is the input.
- Useful for optimization & sensitivity analysis.

#### Why use it?
- Enables gradient-based optimization [@Smith2023].
- Provides insights into parameter effects.
:::

::: {.column width="30%" style="text-align: center; padding-top: 20%; padding-bottom: 20%;}
![](sandia.png)
**Figure: Sandia logo**
:::

::::


## References {#refs}
