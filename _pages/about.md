---
permalink: /
title: "About Me"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

I am a first-year PhD candidate at the [HKUST NLP Group](https://hkust-nlp.github.io/), supervised by [Professor Junxian He](https://jxhe.github.io/). I graduated from Shanghai Jiao Tong University (SJTU) in June 2024 with a B.Eng. degree.

My research focuses on natural language processing and machine learning. I am particularly interested in:
- LLM Reasoning and Reinforcement Learning
- Hallucination in Vision-Language Models (VLM)
- LLM truthfulness and Interpretability

I have been fortunate to work as a Research Intern at MINIMAX (February 2025 - Present), Tencent WXG (June 2024 - September 2024), and Shanghai AI Lab (June 2023 - December 2023).

I received the Zhiyuan Honor Scholarship at Shanghai Jiao Tong University.

Feel free to contact me at jliugi@connect.ust.hk.

## Publications

{% if site.author.googlescholar %}
  <div class="wordwrap">You can also find my articles on <a href="{{site.author.googlescholar}}">my Google Scholar profile</a>.</div>
{% endif %}

{% include base_path %}

<!-- New style rendering if publication categories are defined -->
{% if site.publication_category %}
  {% for category in site.publication_category  %}
    {% assign title_shown = false %}
    {% for post in site.publications reversed %}
      {% if post.category != category[0] %}
        {% continue %}
      {% endif %}
      {% unless title_shown %}
        <h2>{{ category[1].title }}</h2><hr />
        {% assign title_shown = true %}
      {% endunless %}
      {% include archive-single.html %}
    {% endfor %}
  {% endfor %}
{% else %}
  {% for post in site.publications reversed %}
    {% include archive-single.html %}
  {% endfor %}
{% endif %}
