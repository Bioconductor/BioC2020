---
layout: default
schedule:
  - time: 8:00-8:55am
    type: Talk
    speaker: 
    title: Open breakfast meeting
    url:
  - time: 9:00-9:55am
    type: Workshop
    speaker: Ludwig Geistlinger
    title: "200: Functional enrichment analysis of high-throughput omics data"
    url: https://github.com/waldronlab/enrichOmics
  - time: 10:00-10:55am
    type: Workshop
    speaker: Haibo Liu
    title: "200: Best practices for ATAC-seq QC and data analysis"
    url: https://github.com/haibol2016/ATACseqQCWorkshop
  - time: 11:00-11:55am
    type: Workshop
    speaker: Ludwig Geistlinger, Marcel Ramos, Sehyun Oh
    title: "200: Copy number variation analysis with Bioconductor"
    url: https://github.com/waldronlab/CNVWorkshop
  - time: 12:00-12:55pm
    type: Break
    speaker: Birds of a Feather Talks, Talk with the BioC Core Team
    title: 
    url: 
  - time: 1:00-1:55pm
    type: Workshop
    speaker: Charlotte Soneson,  Aaron Lun, Kevin Rue-Albrecht, Federico Marini
    title: "200: Interactive Visualization of SummarizedExperiment Objects with iSEE"
    url: https://github.com/iSEE/iSEEWorkshop2020
  - time: 2:00-2:55pm
    type: Keynote
    speaker: Kylie Bemis
    title: 
    url: 
  - time: 3:00-3:10pm
    type: Talk
    speaker: Daniel Bunis
    title: "dittoSeq: A universal user friendly single-cell and bulk RNA sequencing visualization toolkit"
    url: 
  - time: 3:10-3:20pm
    type: Talk
    speaker: Koen Van den Berge
    title: Interpretation of single-cell RNA-seq trajectories using differential expression and differential progression analysis
    url: 
  - time: 3:20-3:30pm
    type: Talk
    speaker: F. William Townes
    title: Dimension reduction for massive single-cell datasets
    url: 
  - time: 3:30-3:40pm
    type: Talk
    speaker: Lauren Hsu
    title: "corral: A simple and fast approach for dimensionality reduction and data alignment in single-cell data"
    url: 
  - time: 3:40-3:55pm
    type: "Q&A session"
    speaker: "Q&A session"
    title: 
    url:
  - time: 4:00-4:55pm
    type: Workshop
    speaker: Lihua Julie Zhu, Jianhong Ou
    title: "200: CRISPRseek for design target-specific gRNAs for the CRISPR genome editing system including base editor and prime editor"
    url: https://github.com/LihuaJulieZhu/CRISPRseekGUIDEseqBioc2020Workshop/
  - time: 5:00-5:55pm
    type: Workshop
    speaker: Kai Hu, Jianhong Ou
    title: "200: Integrated ChIP-seq Data Analysis Workshop"
    url: https://github.com/hukai916/IntegratedChIPseqWorkshop
---

{% include header.md %}

# Day 2: Tuesday, July 28, 2020

All time is US Eastern Time. All sessions include Q&A time.

{% for s in page.schedule %}

{{ s.time }} | {% if s.type == "Keynote" %} **{{ s.type }}**, {{ s.speaker }} {% elsif s.type == "Talk" %} {{ s.type }}, {{ s.speaker }}, {{ s.title }} {% elsif s.type == "Q&A session" or s.type == "Break" %} {{ s.speaker }} {% elsif s.type == "Workshop" %} {{ s.type }}, {{ s.speaker }}, [{{ s.title }}]({{ s.url }}) {% endif %}

{% endfor %}

