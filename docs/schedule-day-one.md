---
layout: default
schedule:
  - time: 8:30-9:00am
    type: Talk
    speaker: Martin Morgan
    title: Introduction & Welcome
    url:
  - time: 9:00-9:55am
    type: Keynote
    speaker: Rafael Irizarry
    title: Probabilistic Gene Expression Signatures for Single Cell RNA-seq Data
    url:
  - time: 10:00-10:10am
    type: Talk
    speaker: Yi Wang
    title: Co-expression analysis is biased by a mean-correlation relationship
  - time: 10:10-10:20am
    type: Talk
    speaker: Ting Huang
    title: "MSstatsTMT: Statistical detection of differentially abundant proteins in experiments with isobaric labeling and multiple mixtures"
    url:
  - time: 10:20-10:30am
    type: Talk
    speaker: Simina M. Boca
    title: Using the swfdr package to estimate false discovery rates conditional on covariates
    url:
  - time: 10:30-10:40am
    type: Talk
    speaker: Philippe Boileau
    title: Exploring High-Dimensional Biological Data with Sparse Contrastive Principal Component Analysis
    url:
  - time: 10:40-10:55am
    type: "Q&A session"
    speaker: 
    title: 
    url:
  - time: 11:00-11:55am
    type: Workshop
    speaker: Levi Waldron, Sean Davis
    title: "100: Public data resources in Bioconductor"
    url: https://github.com/waldronlab/PublicDataResources
  - time: 12:00-12:55pm
    type: Break
    speaker: Lunch, Posters, BoF
    title: 
    url: 
  - time: 1:00-1:55pm
    type: Workshop
    speaker: Chloe Mirzayi, Levi Waldron
    title: "100: Epidemiology for Bioinformaticians Workshop"
    url: https://github.com/cmirzayi/epiforbioworkshop
  - time: 2:00-2:55pm
    type: Workshop
    speaker: John Lawson
    title: "100: Annotating inter-sample DNA methylation and ATAC-seq variation with COCOA"
    url: https://github.com/databio/cocoa_workshop_bioc2020
  - time: 3:00-3:55pm
    type: Workshop
    speaker: Leonardo Collado-Torres
    title: "100: Human RNA-seq data from recount2 and related packages"
    url: https://github.com/LieberInstitute/recountWorkshop2020/
  - time: 4:00-4:55pm
    type: Workshop
    speaker: James W. MacDonald
    title: "100: Introduction to Bioconductor Annotation Resources"
    url: https://github.com/jmacdon/Bioc2020Anno
  - time: 5:00-5:55pm
    type: Workshop
    speaker: Stefano Mangiola
    title: "100: A Tidy Transcriptomics introduction to RNA-Seq analyses"
    url: https://github.com/stemangiola/bioc_2020_tidytranscriptomics
---

{% include header.md %}

# Day 1: Monday, July 27, 2020

All time is US Eastern Time. All sessions include Q&A time.

{% for s in page.schedule %}

{{ s.time }} | {% if s.type == "Keynote" %} **{{ s.type }}**, {{ s.speaker }} {% elsif s.type == "Talk" %} {{ s.type }}, {{ s.speaker }}, {{ s.title }} {% elsif s.type == "Q&A session" or s.type == "Break" %} {{ s.speaker }} {% elsif s.type == "Workshop" %} {{ s.type }}, {{ s.speaker }}, [{{ s.title }}]({{ s.url }}) {% endif %}

{% endfor %}

