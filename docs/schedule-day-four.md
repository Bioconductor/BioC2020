---
layout: default
schedule:
  - time: 8:00-8:55am
    type: Workshop
    speaker: Peter F. Hickey
    title: "500: Effectively using the DelayedArray framework as a user to support the analysis of large datasets"
    url: https://github.com/PeteHaitch/BioC2020_DelayedArray_workshop
  - time: 9:00-9:55am
    type: Workshop
    speaker: Sehyun Oh
    title: "100: Cloud-based Genomics using Terra/AnVIL"
    url: https://github.com/waldronlab/AnVILWorkshop
  - time: 10:00-10:55am
    type: Workshop
    speaker: Mikhail Dozmorov
    title: "500: Detection of Differentially Interacting Chromatin Regions From Multiple Hi-C Datasets"
    url: https://github.com/mdozmorov/HiCcompareWorkshop
  - time: 11:00-11:55am
    type: Workshop
    speaker: Kayla Interdonato
    title: "500: Material on how to create and submit a package to Bioconductor"
    url: https://github.com/Kayla-Morrell/CreateAPackage
  - time: 12:00-12:55pm
    type: Break
    speaker: Lunch, Posters, PBoF
    title: 
    url: 
  - time: 2:00-2:55pm
    type: Keynote
    speaker: X Shirley Liu
    title: 
    url: 
  - time: 3:00-3:15pm
    type: Talk
    speaker: Anthony Mammoliti
    title: "ORCESTRA: a platform for orchestrating and sharing high-throughput pharmacogenomic analyses"
    url: 
  - time: 3:15-3:30pm
    type: Talk
    speaker: Shraddha Pai
    title: "netDx: Building interpretable patient classifiers by multi-omic data integration and patient similarity networks"
    url: 
  - time: 3:30-3:45pm
    type: Talk
    speaker: Gabriel Odom
    title: "A Global Test for Integrative Pathway Analysis of Multi-omics Data"
    url: 
  - time: 3:45-4:00pm
    type: Talk
    speaker: Ruth Schmidt
    title: "Visualization of multi-omics data in microbiome research"
    url: 
  - time: 4:00-4:55pm
    type: Workshop
    speaker: Anthony Federico
    title: "500: Efficient, Scalable, and Reproducible Enrichment Workflows"
    url: https://github.com/montilab/hypeR-workshop
  - time: 5:00-5:55pm
    type: Workshop
    speaker: Michael Love
    title: "200: Importing alevin scRNA-seq counts into R/Bioconductor"
    url: https://github.com/mikelove/alevin2bioc
---

{% include header.md %}

# Day 4: Thursday, July 30, 2020

All time is US Eastern Time. All sessions include Q&A time.

{% for s in page.schedule %}

{{ s.time }} | {% if s.type == "Keynote" %} **{{ s.type }}** {% else %} {{ s.type }} {% endif %}, {{ s.speaker }}, {% if s.url contains "http" %} [{{ s.title }}]({{ s.url }}) {% else %} {{ s.title }} {% endif %}

{% endfor %}

