---
permalink: /
title: ""
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

{% include base_path %}

# Bespoke CCAs

Congestion Control Algorithms (CCAs) determine how fast or slow senders transmit over the Internet. As a consequence, these algorithms also determine network utilization, performance stability, buffer occupancy and latency, and fairness of network resource allocation. All of these factors play in to whether applications perform as expected. Historically, the Internet was home to only a few CCAs, but today, we see many new CCAs in deployment. In this project, we aim to understand three aspects of this new era of CCA heterogeneity. First (1) we want to understand the benefit of deploying custom “bespoke” CCAs which are tuned to a particular application. Second (2)  we want to measure and evaluate to what extent operators are already deploying new CCAs on the Internet. Third (3) we aim to understand and evaluate how heterogenous CCAs share resources on the Internet, and whether or not we can determine through testing whether a bespoke CCA is “safe” for deployment.





# Publications

{% for post in site.publications reversed %}
  {% if post.selected %}
    {% include single-publication.html post=post %}
  {% endif %}
{% endfor %}