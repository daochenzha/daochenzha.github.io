---
permalink: /
title: "Homepage"
excerpt: "About me"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

Howdy! I am a fourth-year PhD student from the Department of Computer Science at Rice University, working with Dr. [Xia (Ben) Hu](https://cs.rice.edu/~xh37/). Before joining Rice, I was a PhD student at Texas A&M University, working with Dr. Xia (Ben) Hu. I received my Bachelor degree in Computer Science from Wuhan University in 2018, working with Dr. [Chenliang Li](http://www.lichenliang.net/). I was a Research Intern at Facebook, working on automated machine learning systems, in Summer 2021. I was a Research Intern at Seattle AI Lab of Kuai Inc. in Summer 2020, working with Dr. Wenye Ma and Dr. [Ji Liu](http://jiliu-ml.org/).

My research mainly focuses on machine learning and data mining. In particular, I am interested in Automated Machine Learning (AutoML) and Reinforcement Learning (RL). I am also interested in their applications in Anomaly and Outlier Detection, Graph Neural Networks, Time-Series Analysis, Recommender Systems, and Machine Learning Systems, etc.

<h1> Open-Source Projects </h1>
<img src="https://daochenzha.github.io/files/rlcard/logo.jpg" width="200">
<h3 class="archive__item-title" itemprop="headline" style="font-weight:normal;"> RLCard: A Toolkit for Reinforcement Learning in Card Games (<b>>1,300 stars</b>) </h3>
Presented in <b> IJCAI 2020 </b>
<br>
<a href="http://rlcard.org/">[Website]</a>
|
<a href="https://daochenzha.github.io/files/rlcard-a-platform.pdf">[Paper]</a>
|
<a href="https://douzero.org/">[Demo]</a>
|
<a href="https://github.com/datamllab/rlcard">[Code]</a>
|
<a href="https://www.youtube.com/watch?v=krK2jmSdKZc">[Video]</a>
<br>
<img src="https://daochenzha.github.io/files/douzero-gif.gif" width="350">

<img src="https://daochenzha.github.io/files/douzero_logo.jpg" width="200">
<h3 class="archive__item-title" itemprop="headline" style="font-weight:normal;"> DouZero: Mastering DouDizhu with Self-Play Deep Reinforcement Learning (<b>>1,900 stars</b>) </h3>
Presented in <b>ICML 2021</b>
<br>
<a href="https://douzero.org/">[Demo]</a>
|
<a href="https://arxiv.org/abs/2106.06135">[Paper]</a>
|
<a href="https://github.com/kwai/DouZero">[Code]</a>

<img src="https://raw.githubusercontent.com/datamllab/autovideo/main/docs/autovideo_logo.png" width="200">
<h3 class="archive__item-title" itemprop="headline" style="font-weight:normal;"> AutoVideo: An Automated Video Action Recognition System (<b>Newly Released, >100 stars</b>) </h3>
Preprint
<br>
<a href="https://arxiv.org/abs/2108.04212">[Paper]</a>
|
<a href="https://github.com/datamllab/autovideo">[Code]</a>

<img src="https://raw.githubusercontent.com/datamllab/tods/master/docs/img/tods_logo.png" width="200">
<h3 class="archive__item-title" itemprop="headline" style="font-weight:normal;"> TODS: An Automated Time-series Outlier Detection System (<b>>400 stars</b>) </h3>
Presented in <b>AAAI 2021</b>
<br>
<a href="https://tods-doc.github.io/">[Website]</a>
|
<a href="https://arxiv.org/pdf/2009.09822.pdf">[Paper]</a>
|
<a href="https://github.com/datamllab/tods">[Code]</a>
|
<a href="https://www.youtube.com/watch?v=H0bBXuDUe7s">[Video]</a>

<img src="https://daochenzha.github.io/files/pyodds_logo.jpg" width="200">
<h3 class="archive__item-title" itemprop="headline" style="font-weight:normal;"> PyODDS: An End-to-end Outlier Detection System (<b>>100 stars</b>) </h3>
Presented in <b> WWW 2020 </b>
<br>
<a href="http://pyodds.com/">[Website]</a>
|
<a href="http://dczha.com/files/pyodds-an-end.pdf">[Paper]</a>
|
<a href="https://github.com/datamllab/pyodds">[Code]</a>


<h1> Publications </h1>

<a href="https://scholar.google.com/citations?user=jK0NgMcAAAAJ&hl=en&oi=ao"> [Google Schorlar] </a>
<br>
<b> * Equal contribution </b>

{% include base_path %}

{% assign cur_year = "9999" %}
{% for post in site.publications reversed %}
  {% assign dates = post.date | split: "-" %}
  {% assign year = dates.first %}
  {% if year != cur_year %}
    {% assign cur_year = year %}
<h2> {{ year }} </h2>
  {% endif %}
  {% include archive-single.html %}
{% endfor %}

