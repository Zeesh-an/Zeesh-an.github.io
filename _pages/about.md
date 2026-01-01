---
permalink: /
title: "Zeeshan Memon"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

Hi there! I am a second-year Ph.D. student in the Department of Computer Science at Emory University, advised by [Dr. Liang Zhao](https://cs.emory.edu/~lzhao41/). My research focuses on graph machine learning and foundation models for complex networks. I obtained my B.E. in Software Engineering from the National University of Sciences and Technology (NUST), Pakistan, in 2024, where I worked under [Dr. Faisal Shafait](https://scholar.google.com/citations?user=o9RCNZYAAAAJ&hl=en).

I have previously collaborated with CERN, RheinMain University of Applied Sciences, and the Deep Learning Lab (SEECS, NUST) on projects spanning satellite image super-resolution, OCR for low-resource languages and prompt optimization for LLMs.

## Publications

{% include base_path %}
<ul class="pub-list">
{% for post in site.publications reversed %}
  <li>
    <span class="pub-title">{{ post.title }}</span><br />
    <small><span class="pub-venue">{{ post.venue | default: post.category | capitalize }}</span> · {{ post.date | date: '%Y' }}</small>
  </li>
{% endfor %}
</ul>

## Experience
- Visiting Student, Argonne National Laboratory
- ML Research Intern, CERN — 2023 
- ML Research Intern, RheinMain University of Applied Sciences — 2022

## Services

**Conference Reviewer/Program Committee**
- PC Member, IEEE International Conference on Data Science and Advanced Analytics 2025
- PC Member, LLMs4Science @ AAAI 2025
- Reviewer, Workshop on Rethinking Financial Time-Series 2025
- Reviewer, NEGEL Workshop @ NeurIPS 2025
- Reviewer, Assessing World Models @ ICML 2025
- Reviewer, Re-Align Workshop @ ICLR 2025


**Journal Reviewer**
- Reviewer, IEEE Transactions on Big Data (TBD)
