---
marp: true
theme: gaia
_class: lead
footer: '**Tao Xiang | TUM Informatics**'
paginate: true
backgroundImage: url('https://marp.app/assets/hero-background.svg')
# style: |
#   section {
#     background-color: #fff;
#   }
  
---

<!-- ![bg left:40% 80%](https://marp.app/assets/marp.svg) -->

# EffiFormer Workshop

## Intro

---

# Organization

- Day 1: learn Transformer model
- Day 2: learn the related work
- Day 3: learn FlowFormer
- Day 4-7: research and imagination 

---
# Outcome of this w.s.
- learn the cutting-edge models in NLP
- brainstorm with the team and come up with creative ideas
- one idea --> one paper publication
- person who proposes the idea is the first author, others will be ranked according to the contribution

---
![bg right 60%](https://icongr.am/octicons/mark-github.svg)

# GitHub Repo
- model implementation
- experiments

<br>
<br>

#### Welcome Join!

[![Use this as templatess h:1.5em](https://badgen.net/badge/icon/github?icon=github&label)](https://github.com/TUM-EffiFormer)


---

# Introduction
To better understand the the task we are facing, we define the task of **Research Trend Analysis** as follows:


**Definition** (Research Trend Analysis (RTA))
Consider a collection of literature papers $\mathcal{L} = {L_1, L_2, \ldots, L_n}$. The goal of research trend analysis is to identify $k$ research trends $T_1, T_2, \ldots, T_k$. Each research trend $T_i$ is characterized by a trend text $W_i$, which consists of phrases like "reinforcement learning", and a subset of literature papers $C_i \subseteq \mathcal{L}$ (i.e., a cluster) that belong to this trend.




