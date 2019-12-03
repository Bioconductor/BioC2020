---
layout: default
# speakers:
#   - name: Rob Patro
#     inst: Stony Brook University
#     url: http://www.robpatro.com/redesign
#     blurb: "I am an assistant professor in the Computer Science
#       department at Stony Brook University. My main academic interests
#       include computational biology and bioinformatics, machine
#       learning, programming languages, computer graphics, scientific
#       visualization and parallel computation. I also have recreational
#       interests in math, physics, music, politics and video games."

---

{% include header.md %}

BioC2020 highlights current developments within and beyond
the [Bioconductor](https://www.bioconductor.org) project. 


## Key dates

- Jan 9: Registration Opens
- Jan 15: Call for abstracts/applications for talks, early posters, scholarships, workshops
- March 3: Deadline for proposals for talks, workshops, early posters, and travel scholarships
- March 24: Notification of decision
- July 1: Deadline for late posters and for __Birds of a Feather__ meetings
- July 10: Notification of decision for late posters
- July 10: Last day of early registration
- July 29-31: Bioc2020 Meeting, Boston
  - [Community-Developer Day](./schedule-developer-day) July 29:
    provides developers and would-be developers with insights into
    Bioconductor project direction and software development best
    practices.
  - [Main Conference](./schedule-day-two) July 30-31 :
    morning scientific talks and afternoon workshops provide insights
    and tools required for the analysis and comprehension of
    high-throughput genomic data.
  

## Confirmed Speakers

{% for s in page.speakers %}
{% assign imgpath = "images/speakers/" | append: s.name | remove: ' ' | append: '.jpg' %}
<img src="{{ imgpath }}" style="float:right; width:120px; height:150px; object-fit: cover">
### [{{ s.name }}]({{ s.url }}), {{ s.inst }}

> {{ s.blurb }}

{% endfor %}

More information: [workshop@bioconductor.org][contact]

<a href="https://twitter.com/intent/tweet?button_hashtag=bioc2020&ref_src=twsrc%5Etfw"
    class="twitter-hashtag-button"
    data-show-count="false">Tweet #bioc2020</a>

<script async src="https://platform.twitter.com/widgets.js" charset="utf-8"></script>

[contact]: mailto:workshop@bioconductor.org?subject=BioC2020%20question
[survey]: https://forms.gle/eRWv3tdXLvxYT2CYA
