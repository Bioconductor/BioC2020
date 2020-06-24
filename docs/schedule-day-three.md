---
layout: default
schedule:
  - time: 9:00-9:55am
    type: Keynote
    speaker: Corrie Painter
    title: 
    url: 
  - time: 10:00-10:30am
    type: BoF
    speaker: Leonardo Collado-Torres
    title: "CDSB community: efforts to strengthen the R/Bioconductor developer community in Mexico/LatAm and results showcased by regutools"
    url: https://github.com/Bioconductor/BioC2020/issues/67
  - time: 10:30-11:00am
    type: Presentation
    speaker: 
    title: "Presentation of the CAB + Bioc Awards ceremony"
    url: 
  - time: 11:00-11:55am
    type: Workshop
    speaker: Marcel Ramos
    title: "200: Multi-omic Integration and Analysis of cBioPortal and TCGA data with MultiAssayExperiment"
    url: https://github.com/waldronlab/MultiAssayWorkshop
  - time: 12:00-12:55pm
    type: Break
    speaker: Lunch, Posters, PBoF
    title: 
    url: 
  - time: 1:00-1:55pm
    type: Workshop
    speaker: Aedin Culhane
    title: "200: Hitchhikers Guide to PCA; Demystifying dimensionality reduction in R/Bioconductor"
    url: https://github.com/aedin/Frontiers_Supplement
  - time: 2:00-2:55pm
    type: Keynote
    speaker: Fei Chen
    title: 
    url: 
  - time: 3:00-3:15pm
    type: Talk
    speaker: Lukas M. Weber
    title: "Unsupervised analysis of transcriptome-scale spatial gene expression data in the human frontal cortex"
    url: 
  - time: 3:15-3:30pm
    type: Talk
    speaker: Dario Righelli
    title: VisiumExperiment an S4 class for 10x Visium Spatial Gene Expression
    url: 
  - time: 3:30-3:45pm
    type: Talk
    speaker: Lambda Lu
    title: A comparison of spatial transcriptomics methods
    url: 
  - time: 3:45-4:00pm
    type: Talk
    speaker: Ellis Patrick
    title: "Spatial analysis of in situ cytometry data"
    url: 
  - time: 4:00-4:55pm
    type: Workshop
    speaker: Christopher Eeles
    title: "200: Biomarker discovery from high throughput screening datasets"
    url: https://github.com/bhklab/bioc2020workshop
  - time: 5:00-5:55pm
    type: Workshop
    speaker: Qian Liu
    title: "500: Connecting Bioconductor to other bioinformatics tools using Rcwl"
    url: https://github.com/Liubuntu/Bioc2020RCWL
---

{% include header.md %}

# Day 3: Wednesday, July 29, 2020

All time is US Eastern Time. All sessions include Q&A time.

{% for s in page.schedule %}

{{ s.time }} | {% if s.type == "Keynote" %} **{{ s.type }}** {% else %} {{ s.type }} {% endif %}, {{ s.speaker }}, {% if s.url contains "http" %} [{{ s.title }}]({{ s.url }}) {% else %} {{ s.title }} {% endif %}

{% endfor %}

