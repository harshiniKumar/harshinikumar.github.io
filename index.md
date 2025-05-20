---
title: Harshini Kumarasubramanian
page-layout: full
subtitle: "Specialist Programmer, Infosys Ltd"
about:
  id: about-heading
  template: trestles
  image: images/profile.jpg
  image-shape: rounded
  links:
    - text: "{{< fa envelope >}} Mail"
      aria-label: email
      href: "mailto:harshinikumar118@gmail.com"
    - icon: github
      text: GitHub
      aria-label: github
      href: https://github.com/harshiniKumar
    - text: "{{< fa graduation-cap >}} Google Scholar"
      aria-label: google-scholar
      href: https://scholar.google.com/citations?user=vixvH9kAAAAJ&hl=en
    - icon: linkedin
      text: LinkedIn
      aria-label: linkedin
      href: https://www.linkedin.com/in/yourlinkedin/

aliases:
  - /about
editor_options:
  chunk_output_type: console
---

::: {#about-heading}

I am a Specialist Programmer at Infosys Ltd with expertise in machine learning and foundation model development. My work focuses on creating efficient AI solutions that solve real-world problems.

## Research interests

### Foundation Model Training

I specialize in developing and fine-tuning large language models for specific domains. My research explores optimization techniques that reduce computational overhead while maintaining model performance. I'm particularly interested in:

- Efficient training methodologies for large-scale models
- Knowledge distillation and model compression
- Domain adaptation for specialized applications
- Interpretability and bias mitigation in foundation models

### Statistical Modelling and Slow Science

I believe in rigorous methodologies that prioritize reproducibility and scientific integrity over quick results. My approach includes:

- Bayesian methods for uncertainty quantification
- Robust statistical analysis that goes beyond p-values
- Open science practices and transparent research workflows
- Critical evaluation of machine learning methodologies

## Current Projects

- **Efficient LLM Fine-tuning**: Developing techniques to adapt foundation models to specialized domains with minimal computational resources
- **Explainable AI Systems**: Building tools that make complex model decisions more transparent and interpretable
- **Cross-modal Foundation Models**: Exploring the integration of multimodal data in foundation model architectures

## Working together

If you are a scientist who wants to collaborate on ML/AI research or applications, please [reach out to me](mailto:harshinikumar118@gmail.com)!

:::

```{r writing-redirects, echo = FALSE, eval = FALSE}
# NB: this only works for Netlify...
# listing names of post folders
posts <- list.dirs(
  path = here::here("blog"),
  full.names = FALSE,
  recursive = FALSE
  )

# extracting the slugs
slugs <- gsub(".*-(.*)$", "\\1", posts)

# lines to insert to a netlify _redirect file
redirects <- paste0("/post/", slugs, "/ ", "/blog/", posts, "/")

# writing the _redirect file
writeLines(redirects, here::here("docs", "_redirects") )
```