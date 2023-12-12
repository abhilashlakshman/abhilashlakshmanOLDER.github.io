---
layout: page
permalink: /repositories/
title: links of interest
description: My github profile, some important repos, and general links of interest.
nav: true
nav_order: 3
---

### GitHub users

{% if site.data.repositories.github_users %}
<div class="repositories d-flex flex-wrap flex-md-row flex-column justify-content-between align-items-center">
  {% for user in site.data.repositories.github_users %}
    {% include repository/repo_user.html username=user %}
  {% endfor %}
</div>

---

{% if site.repo_trophies.enabled %}
{% for user in site.data.repositories.github_users %}
  {% if site.data.repositories.github_users.size > 1 %}
  <h4>{{ user }}</h4>
  {% endif %}
  <div class="repositories d-flex flex-wrap flex-md-row flex-column justify-content-between align-items-center">
  {% include repository/repo_trophies.html username=user %}
  </div>

  ---

{% endfor %}
{% endif %}
{% endif %}

### GitHub Repositories

{% if site.data.repositories.github_repos %}
<div class="repositories d-flex flex-wrap flex-md-row flex-column justify-content-between align-items-center">
  {% for repo in site.data.repositories.github_repos %}
    {% include repository/repo.html repository=repo %}
  {% endfor %}
</div>
{% endif %}

### My lab affiliations and general sleep and circadian questions you may have
- [Orie Shafer Lab](https://www.shaferlab.org)
- [Sheeba Vasu Lab](https://www.clockclub.org)
- [Sleep and Circadian FAQ](http://www-personal.umich.edu/~ojwalch/sleepfaq/)

### Tools to study what I study
- [Trikinetics](https://trikinetics.com) (The best way to record locomotor activity in insects!)
- [RhythmicAlly](https://github.com/abhilashlakshman/RhythmicAlly) (R-based software to analyse biological timeseries)
- [PHASE](https://github.com/ajlopatkin/PHASE) (MATLAB-based software to analyse _Drosophila_ activity and sleep)

### Academic societies and science education
- [Society for Research on Biological Rhythms (SRBR)](https://srbr.org)
- [European Biological Rhythms Society (EBRS)](https://www.ebrs-online.org)
- [Resonance Journal of Science Education](https://www.ias.ac.in/Journals/Resonance_–_Journal_of_Science_Education/) (An incredibly interesting journal of science education brought to you by the [Indian Academy of Sciences](https://www.ias.ac.in))

### Why the fly is awesome!!
- [Flybase](http://flybase.org)
- [Transgenic fly virtal lab](https://www.biointeractive.org/classroom-resources/transgenic-fly-virtual-lab)
- [The interactive fly](https://www.sdbonline.org/sites/fly/aimain/1aahome.htm)
- [Small fly, BIG Impact - Part 1](https://www.youtube.com/watch?v=qDbJnFLl3kU)
- [Small fly, BIG Impact - Part 2](https://www.youtube.com/watch?v=C9FSf6nhDSc)
