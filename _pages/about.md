---
permalink: /
title: "About Me"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---


I am a first-year Ph.D. student in the **Operations Research Group at the University of Toronto MIE Department**, under the supervision of **Prof. Peyman Mohajerin Esfahani** and **Prof. Nasser Barjesteh**. Prior to joining the University of Toronto, I completed my M.Sc. in Computer Science at the University of Alberta, where I was supervised by [Dr. Xiaoqi Tan](https://xiaoqitan.org/) (see my thesis below). I also worked for one year as a **full-time Research Assistant** in the Department of Computing Science at the **University of Alberta**, working with [Dr. Xiaoqi Tan](https://xiaoqitan.org/) and [Dr. Bo Sun](https://sunbo-online.github.io/). I earned my **B.Sc. in Computer Science** from the **University of Tehran**.

My research focuses on **online optimization** and **mechanism design**, with applications to resource allocation in online markets. My work has appeared in venues such as **WINE**, **ACM SIGMETRICS**, and **The Web Conference**.
---

### Research Interests:
- Decision making under uncertainty
- Combinaotrial optimization and polyhedral methods
- Computational Economics
- Algorithmic game theory and mechanism design

---

### Most Recent Publication
<style>
/* Stronger than the theme's .notice--primary a rules */
.notice--primary .featured-title { 
  font-size: 1.1rem !important;   /* bigger title */
  font-weight: 800;
  color: #161553ff !important;      /* red; change to your brand color */
  margin: 0 0 0.25rem 0;
  line-height: 1.2;
}
.notice--primary .featured-title a {
  color: inherit !important;      /* keep the same color for the link */
  text-decoration: none;
}
.notice--primary .featured-title a:hover {
  text-decoration: underline;
}
</style>

<div class="notice--primary" markdown="1">
{% assign paper_permalink = "/publication/2025-risk-sensitive-online-selection-with-bounded-adaptivity" %}
{% assign pub = site.publications | where: "permalink", paper_permalink | first %}

{% if pub %}
  {% if pub.paperurl %}{% assign link = pub.paperurl %}{% else %}{% assign link = pub.url | relative_url %}{% endif %}

  <h3 class="featured-title">
    <a href="{{ link }}"><span class="thesis-tag">PREPRINT</span>{{ pub.title }}</a>
  </h3>
  {% if pub.authors %}
  **Authors:** {{ pub.authors }}
  {% endif %}

  {% if pub.paperurl %}
  **PDF:** [Download]({{ pub.paperurl }})
  {% endif %}

{% else %}
  *Publication not found. Check the `paper_permalink` and ensure the file is in `/_publications/`.*
{% endif %}
</div>

<div class="notice--primary" markdown="1">
{% assign paper_permalink = "/publication/2025-arxiv-online-rounding-k-rental" %}
{% assign pub = site.publications | where: "permalink", paper_permalink | first %}

{% if pub %}
  {% if pub.paperurl %}{% assign link = pub.paperurl %}{% else %}{% assign link = pub.url | relative_url %}{% endif %}

  <h3 class="featured-title">
    <a href="{{ link }}"><span class="thesis-tag">WWW 2026 (Track: Economics, Online Markets and Human Computation)</span>{{ pub.title }}</a>
  </h3>
  {% if pub.authors %}
  **Authors:** {{ pub.authors }}
  {% endif %}

  {% if pub.paperurl %}
  **PDF:** [Download]({{ pub.paperurl }})
  {% endif %}

{% else %}
  *Publication not found. Check the `paper_permalink` and ensure the file is in `/_publications/`.*
{% endif %}
</div>

<div class="notice--primary" markdown="1">
{% assign paper_permalink = "/publication/2025-thesis-master" %}
{% assign pub = site.publications | where: "permalink", paper_permalink | first %}

{% if pub %}
  {% if pub.paperurl %}{% assign link = pub.paperurl %}{% else %}{% assign link = pub.url | relative_url %}{% endif %}



  <h3 class="featured-title">
    <a href="{{ link }}"><span class="thesis-tag">MASTER THESIS</span>{{ pub.title }}</a>
  </h3>

  <style>
  .thesis-tag{
    display:inline-block; padding:.15rem .45rem; margin-right:.5rem;
    font-size:.75rem; font-weight:700; line-height:1; border-radius:.35rem;
    background:#ffe2a8; color:#7a4d00;
  }
  </style>
  
  {% if pub.authors %}
  **Authors:** {{ pub.authors }}
  {% endif %}

  {% if pub.paperurl %}
  **PDF:** [Download]({{ pub.paperurl }})
  {% endif %}

{% else %}
  *Publication not found. Check the `paper_permalink` and ensure the file is in `/_publications/`.*
{% endif %}
</div>



[Full list of publications →]({{ '/publications/' | relative_url }})


---

### News
{% assign news = site.posts | where_exp:'p','p.categories contains "news"' | sort: 'date' | reverse %}
{% for p in news limit:5 %}
- **{{ p.date | date: "%Y-%m-%d" }}** — [{{ p.title }}]({{ p.url | relative_url }})
{% endfor %}
<a href="{{ '/year-archive/' | relative_url }}">More news →</a>

---


### Contact
Edmonton, Canada · [nekouyan@ualberta.ca](mailto:nekouyan@ualberta.ca) ·
[CV](/files/CV.pdf)
