---
layout: default
usemathjax: true
---
<!-- 
I'm currently a research resident at VinAI Research. 

I am interested in data-efficient and robust machine learning methods. Currently, I mainly focus on the techniques of Active Learning for selecting informative samples, the applications of Bayesian Inference and Distributionally Robust Optimization for enhancing the quality and robustness of ML models.

I am also passionate about deep learning techniques, especially deep generative models like GANs, VAEs, and Normalizing Flows. -->

I'm currently a second-year Ph.D. Student at The University of Iowa.

I'm interested in Machine Learning and its application in general, data-efficient and robust machine learning methods in specific. Currently, I mainly focus on deep generative models (VAEs, GANs) for sequential data with physics information from epidemiology problems. Previously, I worked on different ML topics such as Active Learning techniques, Bayesian Neural Networks, Distributionally Robust Optimization and Fairness problem. 

# Biography

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
Aug. 2014 – Mar. 2019 | Student at Hanoi University of Science and Technology (HUST). I graduated one semester earlier than the five-year standard program with an Excellence Degree of Engineer in Information Systems

" | split: '---' 
%}

{% for milestone in biography %}
{% assign milestone_arr = milestone | strip | split: "|" %}
__<span> {{ milestone_arr[0] | strip }} </span>__ : *{{ milestone_arr[1] | strip}}*
{% endfor %}

# Publications

{% 
assign publications = "

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
Xuan Bui, __Hieu Vu*__, Oanh Nguyen, Khoat Than |
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
- [Bijaya Adhikari](https://cs.uiowa.edu/people/bijaya-adhikari)
- [Viet-Anh Nguyen](https://vietanhnguyen.net)
- [Toan Tran](https://researchers.adelaide.edu.au/profile/toan.m.tran)
- [Khoat Than](https://scholar.google.com.vn/citations?user=z2_6ZRYAAAAJ) 


# Collaborators
- [Man-Chung Yue](https://manchungyue.com/)
- [Gustavo Carneiro](https://cs.adelaide.edu.au/~carneiro/)
- [Xuan Bui](https://scholar.google.com.vn/citations?user=DSLkmeUAAAAJ)