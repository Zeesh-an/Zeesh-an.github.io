---
permalink: /
title: "Zeeshan Memon"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

<button type="button" class="pronounce-btn" id="pronounce-btn" aria-label="Hear how to pronounce my name" title="Hear how to pronounce my name">
  <i class="fas fa-volume-high" aria-hidden="true"></i>
</button>
<audio id="pronounce-audio" src="{{ base_path }}/files/audio/name-pronunciation.m4a" preload="none"></audio>
<script>
  (function () {
    var btn = document.getElementById("pronounce-btn");
    var audio = document.getElementById("pronounce-audio");
    var title = document.querySelector(".page__title");
    if (title) title.appendChild(btn);
    btn.addEventListener("click", function () {
      audio.currentTime = 0;
      audio.play();
    });
    audio.addEventListener("play", function () { btn.classList.add("playing"); });
    audio.addEventListener("ended", function () { btn.classList.remove("playing"); });
  })();
</script>

Hi there! I am a third-year Ph.D. student in the Department of Computer Science at Emory University, advised by [Dr. Liang Zhao](https://cs.emory.edu/~lzhao41/). I obtained my B.E. in Software Engineering from the National University of Sciences and Technology (NUST), Pakistan, in 2024, where I worked under [Dr. Faisal Shafait](https://scholar.google.com/citations?user=o9RCNZYAAAAJ&hl=en).

## Research Interests

<p class="research-lead">I study how agents <strong>learn to improve their decisions</strong> in complex scientific domains where feedback is slow and expensive.</p>

<div class="rcards">
{% for topic in site.data.research %}
  <a class="rcard" href="{{ base_path }}/publications/?topic={{ topic.id }}">
    <span class="rcard-icon"><i class="fas {{ topic.icon }}" aria-hidden="true"></i></span>
    <span class="rcard-title">{{ topic.title }}</span>
    <span class="rcard-text">{{ topic.summary }}</span>
    <span class="rcard-go" aria-hidden="true">&rarr;</span>
  </a>
{% endfor %}
</div>

<div class="open-to">
  <div class="open-to-label">Seeking Spring/Summer 2027 internships</div>
  I am currently seeking <strong>research and applied scientist internships for Spring/Summer 2027</strong>, and I am always open to <strong>research collaborations</strong>. If my work aligns with yours, I would be glad to collaborate or discuss ideas. Feel free to reach out by <a href="mailto:{{ site.author.email }}">email</a>!
</div>

## Experience

<div class="work-list">

  <div class="work-row">
    <img class="work-logo" src="{{ base_path }}/images/logos/microsoft.png" alt="Microsoft" />
    <div class="work-main">
      <div class="work-org">Microsoft Research</div>
      <div class="work-role">Research Intern · Redmond, WA, USA</div>
    </div>
    <div class="work-date">May 2026 – Aug 2026</div>
  </div>

  <div class="work-row">
    <img class="work-logo" src="{{ base_path }}/images/logos/argonne.png" alt="Argonne" />
    <div class="work-main">
      <div class="work-org">Argonne National Laboratory</div>
      <div class="work-role">Visiting Student</div>
    </div>
    <div class="work-date">Oct 2025 – May 2026</div>
  </div>

  <div class="work-row">
    <img class="work-logo" src="{{ base_path }}/images/logos/emory.png" alt="Emory University" />
    <div class="work-main">
      <div class="work-org">MICS Lab, Emory University</div>
      <div class="work-role">Graduate Research Assistant</div>
    </div>
    <div class="work-date">Aug 2024 – Present</div>
  </div>

  <div class="work-row">
    <img class="work-logo" src="{{ base_path }}/images/logos/cern.png" alt="CERN" />
    <div class="work-main">
      <div class="work-org">CERN</div>
      <div class="work-role">ML Research Intern</div>
    </div>
    <div class="work-date">Jun – Aug 2023</div>
  </div>

  <div class="work-row">
    <img class="work-logo" src="{{ base_path }}/images/logos/rheinmain.png" alt="RheinMain" />
    <div class="work-main">
      <div class="work-org">RheinMain University of Applied Sciences</div>
      <div class="work-role">ML Research Intern</div>
    </div>
    <div class="work-date">Jun – Sep 2022</div>
  </div>

</div>

## News

<div class="news-list" id="news-list">
  <div class="news-item">
    <span class="news-date">Oct 2026</span>
    <span class="news-text">Received the NeurIPS 2026 Financial Assistance Award!</span>
  </div>
  <div class="news-item">
    <span class="news-date">Sep 2026</span>
    <span class="news-text"><a href="https://arxiv.org/abs/2611.10627">CONSTRAINER</a> accepted to NeurIPS 2026!</span>
  </div>
  <div class="news-item">
    <span class="news-date">Sep 2026</span>
    <span class="news-text">Passed my Ph.D. Qualifying Exam!</span>
  </div>
  <div class="news-item">
    <span class="news-date">Aug 2026</span>
    <span class="news-text"><a href="https://arxiv.org/abs/2610.02744">EpiWorld: Grounding LLM Policy Agents in Epidemiological World Models</a> accepted to EMNLP 2026 Findings!</span>
  </div>
  <div class="news-item">
    <span class="news-date">Jun 2026</span>
    <span class="news-text">Received the KDD 2026 Student Travel Award.</span>
  </div>
  <div class="news-item">
    <span class="news-date">May 2026</span>
    <span class="news-text"><a href="https://arxiv.org/abs/2605.02026">Towards Systematic Generalization for Power Grid Optimization Problems</a> accepted at KDD 2026!</span>
  </div>
  <div class="news-item">
    <span class="news-date">Apr 2026</span>
    <span class="news-text"><a href="https://arxiv.org/abs/2503.00646">DIPT (Deep Identification of Propagation Trees)</a> accepted at IJCAI 2026!</span>
  </div>
  <div class="news-item">
    <span class="news-date">Apr 2026</span>
    <span class="news-text">Excited to be joining Microsoft as a Research Intern this May — reach out if you'll be in Seattle!</span>
  </div>
  <div class="news-item">
    <span class="news-date">Mar 2026</span>
    <span class="news-text">Two works on <a href="https://openreview.net/forum?id=T5ACq6FQqh">Epidemiology World Model</a> and <a href="https://arxiv.org/abs/2603.04300">Foundation Model for Power Grid Optimization</a> accepted to ICLR workshops!</span>
  </div>
  <div class="news-item">
    <span class="news-date">Aug 2024</span>
    <span class="news-text">Started PhD at Emory University!</span>
  </div>
  <div class="news-item">
    <span class="news-date">Jun 2024</span>
    <span class="news-text"><a href="https://openreview.net/forum?id=d0jQuZe6k0">LLM-Informed Discrete Prompt Optimization</a> accepted at the ICML 2024 Workshop on LLMs and Cognition.</span>
  </div>
  <div class="news-item">
    <span class="news-date">May 2024</span>
    <span class="news-text">Awarded NUST Rector Gold Medal for best Final Year Project in the batch of Software Engineering, and NUST President Gold Medal for highest distinction in the batch of Software Engineering.</span>
  </div>
  <div class="news-item">
    <span class="news-date">Mar 2023</span>
    <span class="news-text">First paper, <a href="https://link.springer.com/chapter/10.1007/978-3-031-41685-9_27">Content-aware Urdu handwriting generation</a>, accepted at ICDAR 2023 (International Conference on Document Analysis and Recognition).</span>
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
<script>
  (function () {
    var list = document.getElementById("news-list");
    if (!list) return;
    var update = function () {
      var atEnd = list.scrollTop + list.clientHeight >= list.scrollHeight - 4;
      list.classList.toggle("at-end", atEnd);
    };
    list.addEventListener("scroll", update);
    update();
  })();
</script>

## Achievements

- Student Travel Award, KDD 2026
- Awarded Rector's Gold Medal for best final-year undergraduate research project
- Awarded Presidential Gold Medal for securing rank one in batch in Bachelors of Software Engineering
- Selected as prestigious Openlab Researcher at CERN from pool of 2000 candidates (1.5% acceptance rate)
- Awarded prestigious MBZUAI undergraduate fully funded research internship
- Awarded DAAD fully funded research internship
- Got NUST Merit Based Scholarship for 8 consecutive semesters

## Teaching & Service

<div class="dense">
<p><strong>Teaching Assistant:</strong> CS 584 Spatial Computing, CS 584 Deep Learning on Graphs, CS 110 Computer Science Fundamentals (Emory University); CS 250 Data Structures and Algorithms (NUST)</p>
<p><strong>Reviewer:</strong> NeurIPS 2026, KDD 2026, IEEE Transactions on Big Data, IEEE Transactions on Computational Social Systems</p>
<p><strong>Program Committee:</strong> IEEE DSAA 2025, LLMs4Science @ AAAI 2025</p>
</div>

<p class="last-updated">Last updated: {{ site.time | date: "%B %Y" }}</p>

<style>
.research-lead {
  font-size: 1.05em;
  line-height: 1.6;
  margin-bottom: 0.4em !important;
}
.rcards {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  gap: 12px;
  margin: 10px 0 20px;
}
.page__content a.rcard {
  position: relative;
  display: flex;
  flex-direction: column;
  padding: 16px 16px 30px;
  border: 1px solid var(--global-border-color);
  border-radius: 10px;
  background: var(--global-bg-color);
  color: var(--global-text-color);
  text-decoration: none;
  transition: border-color 0.2s, box-shadow 0.2s, transform 0.2s;
}
.page__content a.rcard:hover,
.page__content a.rcard:focus-visible {
  border-color: var(--global-link-color);
  box-shadow: 0 6px 18px rgba(0, 0, 0, 0.08);
  transform: translateY(-2px);
}
.rcard-icon {
  display: inline-flex;
  align-items: center;
  justify-content: center;
  width: 36px;
  height: 36px;
  margin-bottom: 12px;
  border-radius: 8px;
  background: rgba(127, 127, 127, 0.1);
  background: color-mix(in srgb, var(--global-link-color) 12%, transparent);
  color: var(--global-link-color);
  font-size: 16px;
}
.rcard-title {
  font-family: "Inter", -apple-system, sans-serif;
  font-weight: 700;
  font-size: 0.98em;
  line-height: 1.3;
}
.rcard-text {
  margin-top: 6px;
  font-size: 0.86em;
  line-height: 1.55;
  color: var(--global-text-color-light);
}
.rcard-go {
  position: absolute;
  right: 14px;
  bottom: 8px;
  font-family: "Inter", -apple-system, sans-serif;
  color: var(--global-link-color);
  opacity: 0;
  transition: opacity 0.2s;
}
.rcard:hover .rcard-go,
.rcard:focus-visible .rcard-go { opacity: 1; }
@media (max-width: 700px) {
  .rcards { grid-template-columns: 1fr; }
}
.pronounce-btn {
  display: inline-flex;
  align-items: center;
  justify-content: center;
  width: 32px;
  height: 32px;
  margin-left: 12px;
  padding: 0;
  vertical-align: middle;
  border: 1px solid var(--global-border-color);
  border-radius: 50%;
  background: var(--global-bg-color);
  color: var(--global-link-color);
  font-size: 15px;
  line-height: 1;
  cursor: pointer;
  transition: background 0.15s, color 0.15s;
}
.pronounce-btn i { font-size: 15px; }
.pronounce-btn:hover,
.pronounce-btn.playing {
  background: var(--global-link-color);
  color: #fff;
}
.dense p {
  margin: 0 0 0.35rem;
  font-size: 0.9em;
  line-height: 1.55;
}
.open-to {
  margin: 16px 0 8px;
  padding: 12px 16px;
  border: 1px solid var(--global-border-color);
  border-left: 4px solid var(--global-link-color);
  border-radius: 6px;
  background: rgba(127,127,127,0.06);
  background: color-mix(in srgb, var(--global-link-color) 8%, var(--global-bg-color));
  box-shadow: 0 1px 4px rgba(0,0,0,0.06);
  font-size: 0.92em;
  line-height: 1.6;
}
.open-to-label {
  margin-bottom: 4px;
  font-size: 0.78em;
  font-weight: 700;
  letter-spacing: 0.06em;
  text-transform: uppercase;
  color: var(--global-link-color);
}
.last-updated {
  margin-top: 28px;
  text-align: right;
  font-size: 0.78em;
  font-style: italic;
  color: var(--global-text-color-light);
}
.page__title {
  font-size: 2.6em;
  font-weight: 800;
  letter-spacing: -0.03em;
  line-height: 1.05;
  margin-bottom: 0.45em;
}
.news-list {
  margin-top: 10px;
  max-height: 230px;
  overflow-y: auto;
  padding-right: 6px;
  -webkit-mask-image: linear-gradient(to bottom, #000 80%, transparent);
          mask-image: linear-gradient(to bottom, #000 80%, transparent);
}
.news-list.at-end {
  -webkit-mask-image: none;
          mask-image: none;
}
.news-list::-webkit-scrollbar { width: 4px; }
.news-list::-webkit-scrollbar-thumb { background: var(--global-border-color); border-radius: 4px; }
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
.work-list { margin-top: 6px; }
.work-row {
  display: flex;
  align-items: center;
  gap: 16px;
  padding: 12px 0;
  border-bottom: 1px solid var(--global-border-color);
}
.work-row:last-child { border-bottom: none; }
.work-logo {
  width: 84px;
  height: 56px;
  object-fit: contain;
  flex-shrink: 0;
  background: #fff;
  border-radius: 4px;
  padding: 3px;
}
.work-main { flex: 1; min-width: 0; }
.work-org { font-weight: 700; font-size: 1em; line-height: 1.35; color: var(--global-text-color); }
.work-role { font-size: 0.85em; margin-top: 2px; color: var(--global-text-color-light); }
.work-date {
  flex-shrink: 0;
  font-size: 0.82em;
  font-weight: 500;
  white-space: nowrap;
  color: var(--global-text-color-light);
}
@media (max-width: 480px) {
  .work-row { flex-wrap: wrap; gap: 4px 12px; }
  .work-date { width: 100%; padding-left: 96px; }
}
</style>
