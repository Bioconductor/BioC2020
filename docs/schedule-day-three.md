---
layout: default
schedule:
  - time: 8:00-8:55am
    type: Talk
    speaker: 
    title: "Presentation of the BioC Commuity Advisory Board and BioC Awards Ceremony"
    url:
  - time: 9:00-9:55am
    type: Keynote
    speaker: Corrie Painter
    title: 
    url: 
  - time: 10:00-10:55am
    type: Talk
    speaker: 
    title: "CDSB community Meeting"
    url: 
  - time: 11:00-11:55am
    type: Workshop
    speaker: Marcel Ramos
    title: "200: MultiAssayExperiment and curatedTCGAData Bioconductor 2020 Workshop"
    url: https://github.com/waldronlab/MultiAssayWorkshop
  - time: 12:00-12:55pm
    type: Break
    speaker: Lunch, Posters, BoF
    title: 
    url: 
  - time: 1:00-1:55pm
    type: Workshop
    speaker: Aedin Culhane
    title: "200: A introduction to principal component analysis"
    url: https://github.com/aedin/PCAworkshop
  - time: 2:00-2:55pm
    type: Keynote
    speaker: Fei Chen
    title: 
    url: 
  - time: 3:00-3:10pm
    type: Talk
    speaker: Lukas M. Weber
    title: "Unsupervised analysis of transcriptome-scale spatial gene expression data in the human frontal cortex"
    url: 
  - time: 3:10-3:20pm
    type: Talk
    speaker: Dario Righelli
    title: VisiumExperiment an S4 class for 10x Visium Spatial Gene Expression
    url: 
  - time: 3:20-3:30pm
    type: Talk
    speaker: Lambda Lu
    title: A comparison of spatial transcriptomics methods
    url: 
  - time: 3:30-3:40pm
    type: Talk
    speaker: Ellis Patrick
    title: "Spatial analysis of in situ cytometry data"
    url: 
  - time: 3:40-3:55pm
    type: "Q&A session"
    speaker: "Q&A session"
    title: 
    url:
  - time: 4:00-4:55pm
    type: Workshop
    speaker: Petr Smirnov, Arvind Mer, Christopher Eeles
    title: "200: A workshop on discovering biomarkers from high throughput response screens"
    url: https://github.com/bhklab/bioc2020workshop
  - time: 5:00-5:55pm
    type: Workshop
    speaker: Qian Liu
    title: "500: Bioconductor toolchain for usage and development of reproducible bioinformatics pipelines in CWL"
    url: https://github.com/Liubuntu/Bioc2020RCWL
---

{% include header.md %}

# Day 3: Wednesday, July 29, 2020

All time is US Eastern Time. All sessions include Q&A time.

{% for s in page.schedule %}

{{ s.time }} | {% if s.type == "Keynote" %} **{{ s.type }}**, {{ s.speaker }} {% elsif s.type == "Talk" %} {{ s.type }}, {{ s.speaker }}, {{ s.title }} {% elsif s.type == "Q&A session" or s.type == "Break" %} {{ s.speaker }} {% elsif s.type == "Workshop" %} {{ s.type }}, {{ s.speaker }}, [{{ s.title }}]({{ s.url }}) {% endif %}

{% endfor %}

