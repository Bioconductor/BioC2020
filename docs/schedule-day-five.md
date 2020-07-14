---
layout: default
schedule:
  - time: 9:00-9:55am
    type: Keynote
    speaker: Caroline Uhler
    title: "Multi-Domain Data Integration: From Observations to Mechanistic Insights"
    url: 
  - time: 10:00-10:10am
    type: Talk
    speaker: Emma Jablonski
    title: Reproducible workflows with the RENKU platform
  - time: 10:10-10:20am
    type: Talk
    speaker: Shian Su
    title: "Analysing DNA Methylation Using Nanopore Long Read Sequencing"
    url:
  - time: 10:20-10:30am
    type: Talk
    speaker: Hena R Ramay
    title: "FemMicro16S: Advancing the science of  women’s health through open data sharing"
    url:
  - time: 10:30-10:40am
    type: Talk
    speaker: Jayaram Kancherla
    title: "Quickly compose custom interactive genomic visualization apps in R/Bioc with epiviz components"
    url:
  - time: 10:40-10:55am
    type: "Q&A session"
    speaker: "Q&A session"
    title: 
    url:
  - time: 11:00-11:55am
    type: Workshop
    speaker: Kelly Street, Koen Van den Berge
    title: "500: Trajectory inference across conditions: differential expression and differential progression"
    url: https://github.com/kstreet13/bioc2020trajectories
  - time: 12:00-12:55pm
    type: Break
    speaker: Lunch, Posters, BoF
    title: 
    url: 
  - time: 2:00-2:55pm
    type: Keynote
    speaker: Aaron Lun
    title: "Making the infrastructure sausage: tales of Bioconductor package development"
    url: 
  - time: 3:00-3:10pm
    type: Talk
    speaker: Charlotte Soneson
    title: "Preprocessing choices affect RNA velocity results for droplet scRNA-seq data"
    url: 
  - time: 3:10-3:20pm
    type: Talk
    speaker: Davide Risso
    title: "Bench pressing differential abundance methods for microbiome data"
    url: 
  - time: 3:20-3:30pm
    type: Talk
    speaker: Anthony Sonrel
    title: "Bench pressing performant single cell RNA-seq preprocessing tools through pipeComp; a general framework for the evaluation of computational pipelines"
    url: 
  - time: 3:30-3:40pm
    type: Talk
    speaker: Stephanie Hicks
    title: "Bench pressing single-cell RNA-sequencing imputation methods"
    url: 
  - time: 3:40-3:55pm
    type: "Q&A session"
    speaker: "Q&A session"
    title: 
    url:
  - time: 4:00-4:55pm
    type: Workshop
    speaker: Natalie Pochet
    title: "200: AMARETTO-Hub: a Knowledge Graph Platform Embedding *AMARETTO Tools for Multimodal and Multiscale Network BioMedicine"
    url: https://github.com/broadinstitute/BioC2020Workshop_AMARETTO-Hub
---

{% include header.md %}

# Day 5: Friday, July 31, 2020

All time is US Eastern Time. All sessions include Q&A time.

{% for s in page.schedule %}

{{ s.time }} | {% if s.type == "Keynote" %} **{{ s.type }}**, {{ s.speaker }}, {{ s.title }} {% elsif s.type == "Talk" %} {{ s.type }}, {{ s.speaker }}, {{ s.title }} {% elsif s.type == "Q&A session" or s.type == "Break" %} {{ s.speaker }} {% elsif s.type == "Workshop" %} {{ s.type }}, {{ s.speaker }}, [{{ s.title }}]({{ s.url }}) {% endif %}

{% endfor %}

