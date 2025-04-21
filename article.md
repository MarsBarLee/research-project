---
title: "Morgan's Marvelous Mutations: Unraveling the Mysteries of Genetic Variation"
abstract: |
  Here we present a templating guide for Research Articles submitted to _The Morganton Scientific_. We use some inspiration from [Thomas Hunt Morgan](https://en.wikipedia.org/wiki/Thomas_Hunt_Morgan), who was a pioneering American geneticist whose work with fruit flies ([Drosophila melanogaster](https://en.wikipedia.org/wiki/Drosophila_melanogaster)) in the early 20th century provided the first solid evidence of genes being carried on chromosomes. This background provides a scaffold for exploring templating in a realistic way, without looking at too much [Lorem Ipsum](https://en.wikipedia.org/wiki/Lorem_ipsum) text. The paper shows analysis in a Jupyter Notebook and uses those in a reproducible manner in the article. Look out for quoted sections that explain the section or other relevant formatting information.

  Your abstract should be between 100-200 words, and introduce a technical synopsis of your paper that includes background, methods, results, and conclusions. You can use the `abstract: |` key in your article frontmatter to write it.
acknowledgments: |
  We thank our school, teachers, and fellow students for their support and encouragement throughout this project.
  Use your acknowledgements section to call out any important contributions or support given to the authors.

  Note, as this was a template article and is _not_ a real scientific study, portions of this paper were created with ChatGPT-4 including images, code and data generation. **Consult your academic guidelines before using ChatGPT in your own work.** Use any form of generative models responsibly and rigorously check the outputs against scientific sources.
---

## Introduction

> Start with a broad picture of the importance and significance of your chosen field while explaining introductory concepts. State the problem and goals that your research will address. Please cite any referenced literature.

Genetic variation is the cornerstone of biological diversity and evolution, underlying the vast array of phenotypes observed within and across species. Understanding the mechanisms and consequences of genetic variation is crucial for unraveling the complexities of life, from individual health and disease susceptibility to the adaptability and survival of species in changing environments. We use some inspiration from [Thomas Hunt Morgan](https://en.wikipedia.org/wiki/Thomas_Hunt_Morgan)[^no-relation], who was a pioneering American geneticist whose work with fruit flies ([Drosophila melanogaster]). Our paper aims to shed light on the phenotypic diversity in three different environments in and around a hypothetical high-school.

% Footnotes are able to be created using the `[^footnote-label]` and then having a definition later:

[^no-relation]: Thomas Morgan has no relation to The Morganton Scientific, his story provides some inspiration for a topic and some associated data-analysis.

The study of genetic variation has witnessed significant advancements in recent years, fueled by technological innovations in genomic sequencing and bioinformatics analysis. We highlight key studies and findings that have contributed to our understanding of genetic variation, its mechanisms, and its implications for both evolutionary biology and human health.

> You can create lists, links and other typography elements, see [typography](https://mystmd.org/guide/typography) for more details.
> Any abbreviations that you use throughout the paper should be explained in your `myst.yml` in the abbreviations section.
> For example, try hovering over CRISPR in the HTML view of the paper!

1. **Genomic Sequencing and Population Genetics**: Recent studies utilizing whole-genome sequencing have provided unprecedented insights into the genetic diversity within and between populations. For example, the 1000 Genomes Project [@10.1038/nmeth.1974] has mapped genetic variations in humans from various parts of the world.

2. **Advances in Gene Editing**: The development of CRISPR-Cas9 [@10.1038/nprot.2013.143] and other gene-editing technologies has opened new avenues for studying genetic variation. Researchers are now able to introduce specific genetic variations into model organisms, providing insights into the functional consequences of these variations and paving the way for potential therapeutic applications.

> Citations can be added with the syntax `[@10.1038/nprot.2013.143]` for a parenthetical citation, or `@10.1038/nprot.2013.143` for a narrative citation.
> To cite multiple articles, use a semicolon, `;`, to separate the list: `[@10.1038/nprot.2013.143; 10.1038/nmeth.1974]`.
> To cite articles or resources without DOIs, use [BibTeX](https://en.wikipedia.org/wiki/BibTeX), and cite the citation-key. See @sec:data-analysis for an example.
> All citations will be created dynamically and there is no need to change the formatting (e.g. [APA Style](https://en.wikipedia.org/wiki/APA_style) or [Chicago](https://en.wikipedia.org/wiki/The_Chicago_Manual_of_Style))

Together, these studies underscore the dynamic nature of genetic variation and its central role in the processes of life. By continuing to explore genetic variation, scientists are unraveling the complex interplay between genetics, evolution, and the environment, with profound implications for understanding biodiversity, disease, and the potential for genetic therapies.

## Materials & Methods

> Describe how you performed your work, referencing methods and procedures of previous research conducted. Focus on the important aspects of your methods and avoid going into too much detail in describing commonly used methods.

In this investigation, we employed a comparative approach to study genetic variation within [Drosophila melanogaster] populations collected from distinct environments. The methodology is structured to facilitate reproducibility and educational engagement while adhering to the rigor of scientific inquiry. This study was conducted following ethical guidelines for the use of model organisms in educational settings, ensuring the humane treatment of [Drosophila melanogaster] throughout the project.

### Sample Collection

[Drosophila melanogaster] specimens were systematically collected from three distinct environments within the school's vicinity: the cafeteria, the biology laboratory, and outdoor green spaces. In @fig:samples, you can see a comically large fly entering the trap that we made. The collection was conducted using simple fruit bait traps over a period of one week to ensure a representative sample of the fly population in each area.

> Figures can be created using the `figure` directive `:::{figure} image-source.png` and then referred to in your document using the `@fig:label`.
> The linked figure will be automatically numbered and linked so you can hover over the preview, (e.g. @fig:samples).
> It is good convention to use the `fig:` prefix for all your figures so when you are reading the markdown, things make sense on what you are referring to!

:::{figure} ./images/fruit-flies.png
:label: fig:samples
Collection methodology for [Drosophila melanogaster] specimens from the biology laboratory. (Note: The image was generated with Dalle, yours should be real!)
:::

Following collection, flies were anesthetized using ice-induced cold shock for easier handling. Morphological traits, specifically eye color and wing size, were documented under stereoscopic microscopes.

% You can label sections to refer to them using the `(label)=` syntax:

(sec:data-analysis)=

### Data Analysis

The observed phenotypic data were classified and recorded in a database. Frequencies of each trait within and across populations were calculated and analyzed to assess the level of genetic variation. Statistical analyses, including [chi-square tests](https://en.wikipedia.org/wiki/Chi-squared_test), were employed to determine the significance of variation between populations, using Jupyter Notebooks an open-source platform that is suitable for educational purposes and advanced research.

> If you choose to do any analysis in Jupyter Notebooks, include them as supporting materials. You can also include any data using a link to the data file directly.

Our overall approach provides a practical and educational framework to engage in scientific research, allowing for the exploration of genetic variation through direct observation and analysis, fostering a deeper understanding of genetic principles, data-science and application to real-world contexts. We used NumPy and Pandas for the analysis [@numpy; @pandas]; the statistical analysis was completed with SciPy [@scipy].

> The paragraph above references citation keys in our BibTeX file: [](./references.bib).

## Results

The investigation into genetic variation among [Drosophila melanogaster] populations from different school environments yielded notable findings, highlighting the influence of environment on phenotypic diversity.

> Create subsections using repeated `###`s, for example, the results section might have multiple sections.

### Phenotypic Variation Among Populations

Morphological examination of the fruit flies revealed distinct phenotypic variations, particularly in eye color and wing size, across the three sampled populations. The cafeteria population exhibited a higher frequency of red-eyed flies (76%) compared to the biology laboratory (58%) and outdoor green spaces (63%). Similarly, variations in wing size were observed, with larger wings being more prevalent in the outdoor population (68%) compared to the cafeteria (49%) and laboratory populations (53%) [See @tab:phenotypic-variation].

> There are a few ways to create tables, you can use a markdown table or a list-table (see [table documentation](https://mystmd.org/guide/tables)).
> @tab:phenotypic-variation shows a markdown table, which is wrapped in a `:::{table}` directive.

:::{table}
:label: tab:phenotypic-variation

Morphological examination of the fruit flies revealed distinct phenotypic variations across the three sampled populations.
The source for this data can be found in [](./fruit_fly_data.csv).

| Environment          | Red-Eyed Flies (%) | Larger Wings (%) |
| -------------------- | ------------------ | ---------------- |
| Cafeteria            | 76%                | 49%              |
| Chemistry Laboratory   | 58%                | 53%              |
| Outdoor Green Spaces | 63%                | 68%              |

:::

### Statistical Analysis of Phenotypic Differences

> Math can be included using the ` ```{math} ` directive with a label, and cross-referenced in the same way as figures.
> Math syntax is written in LaTeX, see the [math documentation](https://mystmd.org/guide/math).
> Inline math is surrounded by dollar-signs, for example, $\chi^2$.

Chi-square tests were conducted to evaluate the statistical significance of the observed differences in phenotypic traits between the fruit fly populations from different environments. We used the chi-squared formula @eq:chi-squared to do the analysis.

```{math}
:label: eq:chi-squared
\chi^2=\sum_{i=1}^{n} \frac{(O_i - E_i)^2}{E_i}
```

The analysis for eye color variation yielded a chi-square statistic of 7.66 with a p-value of 0.022 ($\chi^2$ = 7.66, df = 2, p < 0.05), indicating statistically significant differences in eye color distribution across environments. This suggests that the variation in eye color among the populations could indeed be influenced by their respective environmental conditions.

Similarly, the analysis for wing size variation showed a chi-square statistic of 8.17 with a p-value of 0.017 ($\chi^2$ = 8.17, df = 2, p < 0.05). The differences in wing size across populations are also statistically significant. This finding suggests that, like eye color, the variation in wing size is likely influenced by environmental factors, rather than being a result of random variation.

> When including computational results, ensure to link to your original source in your notebooks or other source files.
> This ensures your research is reproducible.

The results prompt a discussion on the role of environmental factors in shaping genetic variation within populations, which can be seen in @fig:environment. The significant variation in eye color across populations suggests a potential adaptive response to different environmental conditions encountered in each habitat. The lack of significant difference in wing size may indicate that this trait is less sensitive to environmental variation or that the sample size and environmental differences were not sufficient to reveal a significant adaptive pattern.

> In this example, we are linking a figure output from our Jupyter Notebook analysis. See the [documentation on linking outputs](https://mystmd.org/guide/reuse-jupyter-outputs). You will see the line `#| label: nb:analysis` in our Jupyter Notebook.

:::{figure} #nb:analysis
:label: fig:environment
Phenotypic variations in [Drosophila melanogaster] across different environments. It compares the percentage of red-eyed flies and flies with larger wings in the cafeteria, biology laboratory, and outdoor green spaces, providing a visual representation of how these traits vary across the sampled populations.
:::

## Discussion

> Demonstrate how your results are statistically significant and address the research questions posed in the introduction. Interpret your results and the implications of your findings with respect to your field and describe their possible applications.

These findings provide a foundational understanding of how genetic traits can vary within a species due to environmental influences, illustrating the dynamic interplay between genetics and the environment. Furthermore, this investigation highlights the value of using model organisms like [Drosophila melanogaster] in educational settings to explore complex biological concepts through hands-on research. This research project, demonstrates the feasibility of conducting meaningful scientific investigations with limited resources, contributing to the educational experience by fostering critical thinking, data analysis skills, and an appreciation for the principles of genetics and evolution.

## Conclusion

> Recap briefly what was learned from your research and assess the validity of your conclusions. Consider what questions might still remain to be answered and put them in terms of future work and how your research could act as a foundation in addressing these questions.

Our investigation into the phenotypic variations of [Drosophila melanogaster] across different environments has yielded insightful findings on the influence of environmental factors on genetic expression. Through the meticulous collection and analysis of data pertaining to eye color and wing size, we have observed significant variations that suggest a strong environmental component to genetic variation within these populations.

The statistical analysis, particularly the Chi-Squared tests, reinforced these observations by confirming the statistical significance of the differences in phenotypic traits across the environments studied. The findings indicate that the cafeteria, biology laboratory, and outdoor green spaces each present unique conditions that could influence the genetic expression of [Drosophila melanogaster], leading to observable differences in eye color and wing size.

This study contributes to the broader understanding of how environmental factors interact with genetic predispositions to shape the phenotypic outcomes of populations. It underscores the importance of considering both genetic and environmental variables in the study of biological diversity and evolution.

Furthermore, this research demonstrates the feasibility and educational value of conducting genuine scientific inquiries in a high school setting. By engaging students in hands-on research, we not only foster a deeper understanding of genetic principles but also cultivate critical thinking, data analysis skills, and an appreciation for the scientific method.

In conclusion, the observed phenotypic variations in [Drosophila melanogaster] across different environmental settings highlight the dynamic interplay between genetics and the environment. Future studies could expand upon this work by exploring additional environmental variables, employing genetic sequencing to pinpoint specific genetic changes, and incorporating larger sample sizes to enhance the robustness of the findings. Through continued research, we can further unravel the complex mechanisms of genetic variation and environmental adaptation, enriching our comprehension of the natural world.

% It is possible to have links to commonly linked URLs at the bottom of your document:

[Drosophila melanogaster]: https://en.wikipedia.org/wiki/Drosophila_melanogaster
