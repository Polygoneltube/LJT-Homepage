---
layout: archive
title: "CV"
permalink: /cv/
author_profile: true
redirect_from:
  - /resume
---

{% include base_path %}

Education
======
* Ph.D. in Computer Science, Hong Kong University of Science and Technology (HKUST), 2024 - Present
  * Supervisor: Professor Junxian He
  * Research focus: Natural Language Processing and Machine Learning

* B.Eng. in Computer Science, Shanghai Jiao Tong University (SJTU), 2020 - 2024
  * Graduated with honors
  * Received Zhiyuan Honor Scholarship

Research Experience
======
* February 2025 - Present: Research Intern
  * MINIMAX
  * Working on LLM reasoning and reinforcement learning

* June 2024 - September 2024: Research Intern
  * Tencent WXG
  * Advisor: Zifei Shan
  * Working on Vision-Language Models and chart understanding

* June 2023 - December 2023: Research Intern
  * Shanghai AI Lab
  * Advisor: Professor Yu Cheng
  * Working on LLM truthfulness and interpretability

Research Interests
======
* LLM Reasoning and Reinforcement Learning
* Hallucination in Vision-Language Models (VLM)
* LLM truthfulness and Interpretability

Publications
======
  <ul>{% for post in site.publications reversed %}
    {% include archive-single-cv.html %}
  {% endfor %}</ul>
  
Talks
======
  <ul>{% for post in site.talks reversed %}
    {% include archive-single-talk-cv.html  %}
  {% endfor %}</ul>
  
Teaching
======
  <ul>{% for post in site.teaching reversed %}
    {% include archive-single-cv.html %}
  {% endfor %}</ul>
  
Awards and Honors
======
* Zhiyuan Honor Scholarship, Shanghai Jiao Tong University
