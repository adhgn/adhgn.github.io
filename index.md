---
layout: default
title: Welcome
---

# Hello, I'm Reyhan.

I am a student at **UBC** specializing in numerical analysis and data science. My work involves creating efficient algorithms and exploring machine learning model interpretability.

### Technical Skills
* **Languages:** Python (Pandas, Scikit-learn), MATLAB, R.
* **Specialties:** Polynomial interpolation, SVMs, and peer teaching.

### Latest Work
Check out my latest project on [Harmonic Flux](/projects/harmonic-flux), which blends mathematical modeling with vocal arrangement.

### Recent Projects

<ul>
  {% for post in site.posts %}
    <li>
      <a href="{{ post.url | relative_url }}">{{ post.title }}</a> 
      <span>({{ post.date | date: "%B %Y" }})</span>
    </li>
  {% endfor %}
</ul>
