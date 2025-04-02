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
  
format: 
  revealjs:
     theme: theme.scss
     styles:
      - styles.css
     slide-number: c/t
     width: 1600
     height: 900
     margin: 0.05
     echo: true
     format: 
      transition: slide
      incremental: true
      controls: true
      progress: true
      auto-stretch: true  # Ensures content resizes properly
editor: visual
footer: '<img src="sealab.png" style="height: 40px;">'
colorlinks: true
slider: true
incremental: true
bibliography: references.bib
title-slide-attributes:
  data-background-image: "cornell.png"
  data-background-size: auto
  data-background-opacity: "0.4"
  data-background-position: "center 80%"
---

## **BEM Solver in Julia**

:::: {.columns}

::: {.column width="50%"}
#### **Key Features**
- Julia implementation for hydrodynamics.  
- Simplified & parallelizable (free surface) Green’s function [@LIANG201880].  
- First-order gradients via automatic differentiation.  
- GPU-ready influence matrix assembly.  
:::

::: {.column width="50%"}
![](AddedMass_Result.png){width=100%}
**Figure**: Non-dimensional added mass for a hemisphere.  
:::

::::  

---

## **Differentiable Simulation**

:::: {.columns}

::: {.column width="70%"}
##### **Core Idea** {.smaller}
$$\frac{\partial f(\mathbf{x})}{\partial \mathbf{x}}$$ where $f$ is a simulation model and $x$ is the input.

* Useful for optimization & sensitivity analysis.  
* Enables gradient-based optimization.  
* Provides insights into parameter sensitivities.  
:::

::: {.column width="30%"}
![](sandia.png){width=80%}  
**Figure**: Sandia logo  
:::

::::


## MarineHydro.jl
- supports reverse-mode automatic differentiation (aka backpropagation)
- automates discrete adjoint method 
- GPU support (incoming!)
- 100% Julia implementation for hydrodynamics.


## Differentiability Implmentation


## **References** {#refs}
