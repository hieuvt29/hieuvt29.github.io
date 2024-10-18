---
layout: default
usemathjax: true
---


# News

{% 
assign news = "
May. 2024 | Our paper on Efficient and Effective Implicit Dynamic Graph Neural Network has been accepted at KDD 2024.
---
Aug. 2022 | I have started my Ph.D. journey at The University of Iowa.
---
Feb. 2022 | Our paper on Distributionally Robust Fair Principal Components via Geodesic Descents has been accepted at ICLR 2022.

" | split: '---' 
%}

{% for milestone in news %}
{% assign milestone_arr = milestone | strip | split: "|" %}
__<span> {{ milestone_arr[0] | strip }} </span>__ : *{{ milestone_arr[1] | strip}}* 
{% if milestone_arr.size > 2 %}
{% assign subinfo = milestone_arr | slice:2, 6 %}
<ul>
{% for subs in subinfo %}
<li style="font-size: small;"> {{subs | strip}} </li>
{% endfor %}
</ul>
{% endif %}
{% endfor %}


# Biography

I'm currently a third-year Ph.D. Student at The University of Iowa, working with [Prof. Bijaya Adhikari](https://cs.uiowa.edu/people/bijaya-adhikari). Before joining Uiowa, I spent two years as a research resident at VinAI Research and another six months as an AI Engineer, where I was lucky enough to work closely with [Prof. Viet Anh Nguyen](https://vietanhnguyen.net) and [Dr. Toan Tran](https://researchers.adelaide.edu.au/profile/toan.m.tran), and many other talented people. I received my Bachelor's degree in Information Systems from Hanoi University of Science and Technology (HUST) in 2019.

My research interests span machine learning, deep learning, and their applications, with a current focus on graph representation learning and deep generative models (VAEs, GANs, Diffusion) for graph and sequential data. I also have prior experience in active learning, Bayesian neural networks, and distributionally robust optimization. My long-term research goal is to develop data-efficient and robust deep learning models to accelerate their practical applications in real-world scenarios.

<!-- 
{% 
assign biography = "
Aug. 2022 – Present | Ph.D. Student at The University of Iowa.
---
Nov. 2019 – Jun. 2022 | Research Resident & AI Engineer at VinAI Research
---
Jun. 2018 – Apr. 2019 | Software developer at VC Corporation
---
Jun. 2017 – Jun. 2019 | Undergraduate research assistant at Data Science Lab, School of Information and Communication Technology, HUST
---
Aug. 2014 – Mar. 2019 | Student at Hanoi University of Science and Technology (HUST). | I graduated one semester earlier than the standard five-year program with an Excellence Degree of Engineer in Information Systems

" | split: '---' 
%}

{% for milestone in biography %}
{% assign milestone_arr = milestone | strip | split: "|" %}
__<span> {{ milestone_arr[0] | strip }} </span>__ : *{{ milestone_arr[1] | strip}}* 
{% if milestone_arr.size > 2 %}
{% assign subinfo = milestone_arr | slice:2, 6 %}
<ul>
{% for subs in subinfo %}
<li style="font-size: small;"> {{subs | strip}} </li>
{% endfor %}
</ul>
{% endif %}
{% endfor %} -->

# Publications

{% 
assign publications = "
Efficient and Effective Implicit Dynamic Graph Neural Network | 
Yongjian Zhong, __Hieu Vu__, Tianbao Yang, Bijaya Adhikari |
[*KDD, 2024*](https://dl.acm.org/doi/abs/10.1145/3637528.3672026) |
https://arxiv.org/pdb/2406.17894.pdf
---
Distributionally Robust Fair Principal Components via Geodesic Descents |
__Hieu Vu*__, Toan Tran, Man-Chung Yue, Viet Anh Nguyen |
[*ICLR, 2022*](https://openreview.net/forum?id=9NVd-DMtThY) |
https://arxiv.org/pdf/2202.03071.pdf
---
Bayesian Metric Learning for Robust Training of Deep Models under Noisy Labels |
__Hieu Vu*__, Toan Tran, Gustavo Carneiro |
*preprint, 2020* |
pdfs/2020_BDML.pdf
---
MAP Estimation With Bernoulli Randomness, and Its Application to Text Analysis and Recommender Systems |
Xuan Bui, __Hieu Vu__, Oanh Nguyen, Khoat Than |
*IEEE Access, 2020* |
https://ieeexplore.ieee.org/iel7/6287639/8948470/09138369.pdf

" | split: '---' 
%}


{% for pub in publications %}
{% assign pub_arr = pub | strip | split: "|" %}
__<span style='font-size: 20px'> {{ pub_arr[0] | strip }} </span>__ <br> *{{ pub_arr[1] | strip}}* <br> {{ pub_arr[2] | strip}} - [PDF]({{ pub_arr[3] | strip }})<br>
{% endfor %}



# Awards

__Excellence scholarship for the academic year of 2018 − 2019__ <br>
*Granted for top 1% students with highest CPA of School of Information and Communication Technology, HUST*

# Advisors
- Aug. 2022 - present: [Bijaya Adhikari](https://cs.uiowa.edu/people/bijaya-adhikari)
- May. 2021 – Jan. 2022: [Viet-Anh Nguyen](https://vietanhnguyen.net)
- Nov. 2019 – Jan. 2022: [Toan Tran](https://researchers.adelaide.edu.au/profile/toan.m.tran)
- Jun. 2017 – Jun. 2019: [Khoat Than](https://scholar.google.com.vn/citations?user=z2_6ZRYAAAAJ) 

# Collaborators
- [Yongjian Zhong](https://yongjian16.github.io/)
- [Akash Choudhuri](https://soothysay.github.io/)
- [Man-Chung Yue](https://manchungyue.com/)
- [Gustavo Carneiro](https://cs.adelaide.edu.au/~carneiro/)
- [Xuan Bui](https://scholar.google.com.vn/citations?user=DSLkmeUAAAAJ)
