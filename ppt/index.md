---
marp: true
title: Developing a Literature Research Tool that Automatically Search Literature and Summarize the Research Trends
description: IDP Report by Tao Xiang
paginate: true
footer: '**fml** - Lehrstuhl für Fördertechnik Materialfluss Logistik | TUM School of Engineering and Design | Technische Universität München'
---

<style>

  footer {
    font-family: 'Arial', sans-serif; /* 设置字体 */
    font-size: 14px; /* 设置字体大小 */
    /* font-weight: bold; 设置字体粗细 */
    color: #333; /* 设置字体颜色 */
  }
  section {
    display: flex;
    justify-content: flex-start;
    align-items: flex-start;
    text-align: left;
    font-size: 14px; /* 设置字体大小 */
  }
  h1 {
    color: #000; /* 设置h1的字体颜色为黑色 */
    font-size: 30px; /* 设置字体大小 */
  }

  h2 {
    color: #0065bd; /* 设置h2的字体颜色为#0065bd */
    font-size: 20px; /* 设置字体大小 */
  }

  h3 {
    color: #0065bd; /* 设置h2的字体颜色为#0065bd */
    font-size: 25px; /* 设置字体大小 */
  }

  h4 {
    color: #000; /* 设置h2的字体颜色为#0065bd */
    font-size: 20px; /* 设置字体大小 */
  }
   
</style>
<link rel="stylesheet" type="text/css" href="./assets/timeline.css">
<link rel="stylesheet" type="text/css" href="./assets/toc.css">
<!-- <link rel="stylesheet" type="text/css" href="./assets/test.css"> -->





![bg](./images/cover.png)

---
<!-- page 2 -->

![bg](./images/content.png)
# Table of Contents

### 1. Motivation
### 2. Introduction
### 3. Framework Design
### 4. Evaluation & Results
### 5. Limitations & Future Work

---
<!-- page 3 -->
![bg](./images/content.png)
# Table of Contents


### <div class ="highlight-wrapper"><div class="highlight-container"><div class="highlight"> 1. Motivation</div></div></div>
### 2. Introduction
### 3. Framework Design
### 4. Evaluation & Results
### 5. Limitations & Future Work

---
![bg](./images/content.png)
# Motivation
<ul class="timeline">
  <li class="timeline-item">
    <div class="timeline-marker"></div>
    <div class="timeline-content">
      <h4>Research trends are important</h4>
      By researching trends, we can stay ahead of the curve and ensure that our work is always <b>cutting-edge</b>.
    </div>
  </li>
</ul>

---
![bg](./images/content.png)
# Motivation
<ul class="timeline">
  <li class="timeline-item">
    <div class="timeline-marker"></div>
    <div class="timeline-content">
      <h4>Research trends are important</h4>
      By researching trends, we can stay ahead of the curve and ensure that our work is always <b>cutting-edge</b>.
    </div>
  </li>

  <li class="timeline-item">
    <div class="timeline-marker"></div>
    <div class="timeline-content">
      <h4>Challenges in identifying research trends</h4>
<ul>
  <li><b>Lack of standardization</b>: Research data is often presented in different formats and with different terminologies, making it difficult to compare and analyze.</li>
  <li><b>Information overload</b>: With the sheer volume of research being produced every day, it can be difficult to know where to start looking for trends.</li>
  <li><b>Noise in the data</b>: Not all research is equally important or reliable, and it can be difficult to filter out the irrelevant or low-quality studies.</li>
  <li><b>Changing landscape</b>: Research trends can shift rapidly in response to new discoveries and technologies, making it difficult to keep up with the latest developments.</li>
</ul>
    </div>
  </li>
</ul>

---
![bg](./images/content.png)
# Motivation
<ul class="timeline">
  <li class="timeline-item">
    <div class="timeline-marker"></div>
    <div class="timeline-content">
      <h4>Research trends are important</h4>
      By researching trends, we can stay ahead of the curve and ensure that our work is always <b>cutting-edge</b>.
    </div>
  </li>

  <li class="timeline-item">
    <div class="timeline-marker"></div>
    <div class="timeline-content">
      <h4>Challenges in identifying research trends</h4>
<ul>
  <li><b>Lack of standardization</b>: Research data is often presented in different formats and with different terminologies, making it difficult to compare and analyze.</li>
  <li><b>Information overload</b>: With the sheer volume of research being produced every day, it can be difficult to know where to start looking for trends.</li>
  <li><b>Noise in the data</b>: Not all research is equally important or reliable, and it can be difficult to filter out the irrelevant or low-quality studies.</li>
  <li><b>Changing landscape</b>: Research trends can shift rapidly in response to new discoveries and technologies, making it difficult to keep up with the latest developments.</li>
</ul>
    </div>
  </li>

  <li class="timeline-item">
    <div class="timeline-marker"></div>
    <div class="timeline-content">
      <h4>The need for an automated framework</h4>
      Automated literature search and analysis based on <b>machine learning</b> can save time and resources while ensuring accuracy.
    </div>
  </li>
</ul>

---



![bg](./images/content.png)
# Table of Contents


### 1. Motivation
### <div class ="highlight-wrapper"><div class="highlight-container"><div class="highlight"> 2. Introduction</div></div></div>
### 3. Framework Design
### 4. Evaluation & Results
### 5. Limitations & Future Work

---
![bg](./images/content.png)

# Introduction

---
![bg](./images/content.png)

# Table of Contents


### 1. Motivation
### 2. Introduction
### <div class ="highlight-wrapper"><div class="highlight-container"><div class="highlight"> 3. Framework Design</div></div></div>
### 4. Evaluation & Results
### 5. Limitations & Future Work

---
![bg](./images/content.png)
# Table of Contents


### 1. Motivation
### 2. Introduction
### 3. Framework Design
### <div class ="highlight-wrapper"><div class="highlight-container"><div class="highlight"> 4. Evaluation & Results</div></div></div>
### 5. Limitations & Future Work

---
![bg](./images/content.png)
# Table of Contents


### 1. Motivation
### 2. Introduction
### 3. Framework Design
### 4. Evaluation & Results
### <div class ="highlight-wrapper"><div class="highlight-container"><div class="highlight"> 5. Limitations & Future Work</div></div></div>
