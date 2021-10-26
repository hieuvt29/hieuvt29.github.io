---
layout: default
usemathjax: true
---

I'm currently a research resident at VinAI Research. 

I am interested in machine learning methods for limited/corrupted supervision data, which is a common scenario due to the expensive labeling costs. Currently, I mainly focus on the techniques of Active Learning for fully exploiting annotated data; Bayesian Inference framework, Self-Supervised learning and Distributionally Robust Optimization for improving the robustness of ML models. 

I am also passionate about deep learning techniques, especially deep generative models like GANs, VAEs, and Normalizing Flows.

# Biography

{% 
assign biography = "
Nov. 2019 – Present | Research Resident at VinAI Research
---
Jun. 2018 – Apr. 2019 | Software developer at VC Corporation
---
Jun. 2017 – Jun. 2019 | Undergraduate research assistant at Data Science Lab, School of Information and Communication Technology, HUST
---
Aug. 2014 – Mar. 2019 | Undergraduate students at Hanoi University of Science and Technology (HUST)

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
__*Hieu Vu__, Toan Tran, Man-Chung Yue, Viet Anh Nguyen |
*preprint, 2021* |
pdfs/2021_RFPCA.pdf
---
Bayesian Metric Learning for Robust Training of Deep Models under Noisy Labels |
__*Hieu Vu__, Toan Tran, Gustavo Carneiro |
*preprint, 2020* |
pdfs/2020_BDML.pdf
---
MAP Estimation With Bernoulli Randomness, and Its Application to Text Analysis and Recommender Systems |
Xuan Bui, __*Hieu Vu__, Oanh Nguyen, Khoat Than |
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

# Mentors
- [Viet-Anh Nguyen]()
- [Toan Tran]()
- [Khoat Than]() 


# Collaborators
- [Man-Chung Yue]()
- [Gustavo Carneiro]()
- [Xuan Bui]()