---
permalink: /
title: "Zeeshan Memon"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

Hi there! I am a second-year Ph.D. student in the Department of Computer Science at Emory University, advised by [Dr. Liang Zhao](https://cs.emory.edu/~lzhao41/). My research focuses on graph machine learning and foundation models for complex networks. I obtained my B.E. in Software Engineering from the National University of Sciences and Technology (NUST), Pakistan, in 2024, where I worked under [Dr. Faisal Shafait](https://scholar.google.com/citations?user=o9RCNZYAAAAJ&hl=en).

## News

<div class="news-scroll">
  <div class="news-item">
    <span class="news-date">May 2026</span>
    <span class="news-text">Towards Systematic Generalization for Power Grid Optimization Problems accepted at KDD 2026!</span>
  </div>
  <div class="news-item">
    <span class="news-date">Apr 2026</span>
    <span class="news-text">DIPT (Deep Identification of Propagation Trees) accepted at IJCAI 2026!</span>
  </div>
  <div class="news-item">
    <span class="news-date">Apr 2026</span>
    <span class="news-text">Excited to be joining Microsoft as a Research Intern this May — reach out if you'll be in Seattle!</span>
  </div>
  <div class="news-item">
    <span class="news-date">Mar 2026</span>
    <span class="news-text">Two works on Epidemiology World Model and Foundation Model for Power Grid Optimization accepted to ICLR workshops!</span>
  </div>
  <div class="news-item">
    <span class="news-date">Aug 2024</span>
    <span class="news-text">Started PhD at Emory University!</span>
  </div>
  <div class="news-item">
    <span class="news-date">Jun 2024</span>
    <span class="news-text">Paper accepted at the ICML 2024 Workshop on LLMs and Cognition.</span>
  </div>
  <div class="news-item">
    <span class="news-date">May 2024</span>
    <span class="news-text">Awarded NUST Rector Gold Medal for best Final Year Project in the batch of Software Engineering, and NUST President Gold Medal for highest distinction in the batch of Software Engineering.</span>
  </div>
  <div class="news-item">
    <span class="news-date">Mar 2023</span>
    <span class="news-text">First paper accepted at ICDAR 2023 (International Conference on Document Analysis and Recognition).</span>
  </div>
  <div class="news-item">
    <span class="news-date">Mar 2023</span>
    <span class="news-text">Selected for CERN Openlab — heading to Geneva!</span>
  </div>
  <div class="news-item">
    <span class="news-date">Feb 2022</span>
    <span class="news-text">Selected for DAAD-funded research internship at RheinMain University of Applied Sciences.</span>
  </div>
</div>

## Experience

<div class="exp-cards">

  <div class="exp-card exp-card-with-logo">
    <img class="exp-logo" src="{{ base_path }}/images/logos/microsoft.png" alt="Microsoft" />
    <div class="exp-card-body">
      <div class="exp-card-header">
        <span class="exp-role">Research Intern</span>
        <span class="exp-date">May 2026 – Aug 2026</span>
      </div>
      <div class="exp-org">Microsoft Research, Redmond, WA, USA</div>
    </div>
  </div>

  <div class="exp-card exp-card-with-logo">
    <img class="exp-logo" src="{{ base_path }}/images/logos/argonne.png" alt="Argonne" />
    <div class="exp-card-body">
      <div class="exp-card-header">
        <span class="exp-role">Visiting Student</span>
        <span class="exp-date">Oct 2025 – May 2026</span>
      </div>
      <div class="exp-org">Argonne National Laboratory</div>
    </div>
  </div>

  <div class="exp-card exp-card-with-logo">
    <img class="exp-logo" src="{{ base_path }}/images/logos/cern.png" alt="CERN" />
    <div class="exp-card-body">
      <div class="exp-card-header">
        <span class="exp-role">ML Research Intern</span>
        <span class="exp-date">Jun – Aug 2023</span>
      </div>
      <div class="exp-org">CERN</div>
    </div>
  </div>

  <div class="exp-card exp-card-with-logo">
    <img class="exp-logo" src="{{ base_path }}/images/logos/rheinmain.png" alt="RheinMain" />
    <div class="exp-card-body">
      <div class="exp-card-header">
        <span class="exp-role">ML Research Intern</span>
        <span class="exp-date">Jun – Sep 2022</span>
      </div>
      <div class="exp-org">RheinMain University of Applied Sciences</div>
    </div>
  </div>

</div>

## Publications

{% include base_path %}
<div class="exp-cards">
{% for post in site.publications reversed %}
  <div class="exp-card">
    <div class="exp-card-header">
      <span class="exp-role">{{ post.title }}</span>
      <span class="exp-date">{{ post.date | date: '%Y' }}</span>
    </div>
    <div class="exp-org">{% if post.venue %}{{ post.venue }}{% else %}{{ post.category | capitalize }}{% endif %}{% if post.paperurl %} <a class="paper-tag" href="{{ post.paperurl }}">Paper</a>{% endif %}</div>
    {% if post.authors %}<div class="exp-authors">{{ post.authors | replace: "Zeeshan Memon", "<span class='self-author'>Zeeshan Memon</span>" }}</div>{% endif %}
  </div>
{% endfor %}
</div>

## Achievements

- Student Travel Award, KDD 2026
- Awarded Rector's Gold Medal for best final-year undergraduate research project
- Awarded Presidential Gold Medal for securing rank one in batch in Bachelors of Software Engineering
- Selected as prestigious Openlab Researcher at CERN from pool of 2000 candidates (1.5% acceptance rate)
- Awarded prestigious MBZUAI undergraduate fully funded research internship
- Awarded DAAD fully funded research internship
- Got NUST Merit Based Scholarship for 8 consecutive semesters


## Services

**Conference Reviewer/Program Committee**
- PC Member, IEEE International Conference on Data Science and Advanced Analytics 2025
- PC Member, LLMs4Science @ AAAI 2025
- Reviewer, NeurIPS 2026
- Reviewer, KDD 2026


**Journal Reviewer**
- Reviewer, IEEE Transactions on Big Data
- Reviewer, IEEE Transactions on Computational Social Systems

<p class="last-updated">Last updated: {{ site.time | date: "%B %Y" }}</p>

<style>
.last-updated {
  margin-top: 28px;
  text-align: right;
  font-size: 0.78em;
  font-style: italic;
  color: var(--global-text-color-light);
}
.news-scroll {
  max-height: 180px;
  overflow-y: auto;
  display: flex;
  flex-direction: column;
  gap: 0;
  margin-top: 10px;
}
.news-scroll::-webkit-scrollbar { width: 4px; }
.news-scroll::-webkit-scrollbar-thumb { background: var(--global-border-color); border-radius: 4px; }
.news-item {
  display: flex;
  gap: 14px;
  align-items: baseline;
  padding: 5px 0;
  font-size: 0.88em;
  line-height: 1.5;
}
.news-date {
  min-width: 62px;
  font-weight: 600;
  font-size: 0.82em;
  color: var(--global-text-color-light);
  white-space: nowrap;
}
.news-text { color: var(--global-text-color); }
.exp-cards { display: flex; flex-direction: column; gap: 8px; margin-top: 10px; }
.exp-card-with-logo {
  display: flex;
  align-items: center;
  gap: 14px;
}
.exp-logo {
  width: 72px;
  height: 48px;
  object-fit: contain;
  flex-shrink: 0;
  border-radius: 6px;
  background: #fff;
  padding: 4px;
  border: 1px solid var(--global-border-color);
}
.exp-card-body { flex: 1; min-width: 0; }
.exp-card {
  border: 1px solid var(--global-border-color);
  border-top: 3px solid var(--global-dark-border-color);
  border-radius: 6px;
  padding: 12px 16px;
  background: var(--global-bg-color);
  box-shadow: 0 1px 4px rgba(0,0,0,0.06);
  transition: box-shadow 0.2s ease, transform 0.2s ease;
}
.exp-card:hover {
  box-shadow: 0 4px 12px rgba(0,0,0,0.1);
  transform: translateY(-1px);
}
.exp-card-header {
  display: flex;
  justify-content: space-between;
  align-items: flex-start;
  flex-wrap: wrap;
  gap: 4px;
}
.exp-role { font-weight: 600; font-size: 0.95em; line-height: 1.4; }
.exp-date {
  font-size: 0.78em;
  color: var(--global-text-color-light);
  white-space: nowrap;
  font-weight: 500;
  margin-top: 2px;
}
.exp-org {
  font-size: 0.85em;
  margin-top: 5px;
  color: var(--global-text-color-light);
  display: flex;
  align-items: center;
  gap: 6px;
  flex-wrap: wrap;
}
.exp-authors {
  font-size: 0.8em;
  margin-top: 6px;
  color: var(--global-text-color-light);
  line-height: 1.5;
}
.exp-bullets {
  margin: 8px 0 0 0;
  padding-left: 18px;
  font-size: 0.85em;
  color: var(--global-text-color);
  line-height: 1.55;
}
.exp-bullets li { margin-bottom: 3px; }
.self-author { font-weight: 700; text-decoration: underline; color: var(--global-text-color); }
.paper-tag {
  display: inline-block;
  font-size: 0.75em;
  padding: 1px 8px;
  border-radius: 20px;
  border: 1px solid var(--global-link-color);
  color: var(--global-link-color) !important;
  text-decoration: none !important;
  font-weight: 500;
  transition: background 0.15s, color 0.15s;
}
.paper-tag:hover { background: var(--global-link-color); color: #fff !important; }
</style>
