---
permalink: /
title:
author_profile: false
redirect_from:
  - /about/
  - /about.html
---

{% assign featured_publications = site.publications | sort: "date" | reverse %}
{% assign featured_projects = site.mini_projects | sort: "date" | reverse %}

<div class="landing-page">
  <section class="landing-page__hero">
    <div class="landing-page__hero-copy">
      <p class="landing-page__eyebrow">PhD Student in Statistics · CUHK</p>
      <h1 class="landing-page__headline">Ting Tin (Martin) Ma</h1>
      <p class="landing-page__lead">
        I work on high-frequency financial data, change-point detection, and
        non-parametric statistics for dependent and high-dimensional settings.
      </p>
      <p class="landing-page__summary">
        My current research focuses on jump detection and inference under infill
        asymptotics, with a broader interest in statistically rigorous methods for
        complex time series and modern data problems.
      </p>
      <div class="landing-page__actions">
        <a class="landing-page__button landing-page__button--primary" href="{{ '/publications/' | relative_url }}">View Publications</a>
        <a class="landing-page__button" href="{{ '/cv/' | relative_url }}">Open CV</a>
        <a class="landing-page__button" href="mailto:martinmtt@link.cuhk.edu.hk">Email</a>
      </div>
      <ul class="landing-page__highlights">
        <li>Vice-Chancellor's HKPFS Scholarship recipient</li>
        <li>Research in jump testing for high-frequency data</li>
        <li>Background spanning statistics, mathematics, and finance</li>
      </ul>
    </div>
    <div class="landing-page__portrait">
      <img src="{{ '/images/CV_photo.png' | relative_url }}" alt="Portrait of Ting Tin Martin Ma">
      <div class="landing-page__portrait-note">
        <span>Department of Statistics and Data Science</span>
        <span>The Chinese University of Hong Kong</span>
      </div>
    </div>
  </section>

  <section class="landing-page__section">
    <div class="landing-page__section-heading">
      <p class="landing-page__section-label">Focus</p>
      <h2>Research themes</h2>
    </div>
    <div class="landing-page__grid landing-page__grid--three">
      <article class="landing-page__card">
        <h3>High-frequency econometrics</h3>
        <p>
          Methods for detecting and testing jumps in noisy, irregularly observed
          financial return data.
        </p>
      </article>
      <article class="landing-page__card">
        <h3>Dependent high-dimensional data</h3>
        <p>
          Change-point detection and inference for multivariate time series where
          classical independence assumptions are not appropriate.
        </p>
      </article>
      <article class="landing-page__card">
        <h3>Non-parametric methodology</h3>
        <p>
          Distribution-free and semi-parametric tools designed to stay reliable in
          realistic data settings.
        </p>
      </article>
    </div>
  </section>

  <section class="landing-page__section">
    <div class="landing-page__section-heading">
      <p class="landing-page__section-label">Selected Work</p>
      <h2>Recent publications and projects</h2>
    </div>
    <div class="landing-page__grid landing-page__grid--two">
      <div class="landing-page__panel">
        <div class="landing-page__panel-head">
          <h3>Publications</h3>
          <a href="{{ '/publications/' | relative_url }}">See all</a>
        </div>
        <div class="landing-page__stack">
          {% for post in featured_publications limit:2 %}
          <article class="landing-page__work-item">
            <p class="landing-page__meta">{{ post.date | date: "%Y" }} · {{ post.venue }}</p>
            <h4><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h4>
            <p>{{ post.authors }}</p>
          </article>
          {% endfor %}
        </div>
      </div>
      <div class="landing-page__panel">
        <div class="landing-page__panel-head">
          <h3>Mini Projects</h3>
          <a href="{{ '/mini-projects/' | relative_url }}">Browse archive</a>
        </div>
        <div class="landing-page__stack">
          {% for project in featured_projects limit:3 %}
          <article class="landing-page__work-item">
            <p class="landing-page__meta">{{ project.date | date: "%Y" }} · {{ project.venue }}</p>
            <h4><a href="{{ project.url | relative_url }}">{{ project.title }}</a></h4>
            <p>{{ project.content | markdownify | strip_html | strip_newlines | truncate: 140 }}</p>
          </article>
          {% endfor %}
        </div>
      </div>
    </div>
  </section>

  <section class="landing-page__section">
    <div class="landing-page__section-heading">
      <p class="landing-page__section-label">Background</p>
      <h2>Academic path and recognition</h2>
    </div>
    <div class="landing-page__grid landing-page__grid--two">
      <div class="landing-page__panel">
        <h3>Academic background</h3>
        <ul class="landing-page__timeline">
          <li>
            <span class="landing-page__timeline-year">2024-2027</span>
            <div>
              <strong>PhD in Statistics</strong>
              <p>The Chinese University of Hong Kong, supervised by Prof. Chan Kin Wai.</p>
            </div>
          </li>
          <li>
            <span class="landing-page__timeline-year">2024</span>
            <div>
              <strong>MPhil in Risk Management Science</strong>
              <p>The Chinese University of Hong Kong.</p>
            </div>
          </li>
          <li>
            <span class="landing-page__timeline-year">2022</span>
            <div>
              <strong>BSc in Risk Management Science</strong>
              <p>First Class Honours, with a minor in Statistics and Mathematics.</p>
            </div>
          </li>
        </ul>
      </div>
      <div class="landing-page__panel">
        <h3>Awards and honors</h3>
        <ul class="landing-page__compact-list">
          <li>CUHK Vice-Chancellor's HKPFS Scholarship, 2024-2027</li>
          <li>Poster Presentation Award, Merit, Science Faculty Postgraduate Research Day, 2023-2024</li>
          <li>Best Teaching Assistant Award, Department of Statistics, CUHK, 2022-2023</li>
          <li>Bank of East Asia Scholarship, 2021-2022</li>
          <li>Department of Statistics Scholarship, CUHK, 2021-2022</li>
          <li>Dean's List, 2019-2020 and 2020-2021</li>
        </ul>
      </div>
    </div>
  </section>

  <section class="landing-page__section landing-page__section--contact">
    <div class="landing-page__section-heading">
      <p class="landing-page__section-label">Contact</p>
      <h2>Open to research conversations and collaboration</h2>
    </div>
    <div class="landing-page__contact">
      <p>
        The best way to reach me is by email at
        <a href="mailto:martinmtt@link.cuhk.edu.hk">martinmtt@link.cuhk.edu.hk</a>.
        You can also find campus and contact details on the <a href="{{ '/contact/' | relative_url }}">contact page</a>.
      </p>
    </div>
  </section>
</div>
