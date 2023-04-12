---
marp: true
footer: "**fml** - Lehrstuhl für Fördertechnik Materialfluss Logistik | TUM School of Engineering and Design | Technische Universität München"
paginate: True
_class: lead
backgroundImage: url('./images/content.png')


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

.highlight-wrapper {
    margin-bottom: 1.25em; /* 添加底部边距，可根据需要调整 */
  }

   .highlight-container {
    position: absolute;
    left: 0;
    right: 0;
    background-color: #0065bd; /* 设置背景颜色为蓝色 */
    padding-left: 3.17em; /* 添加左边距，可根据需要调整 */
    padding-bottom: 0.2em; /* 添加左边距，可根据需要调整 */
    display: flex; /* 设置为弹性布局 */
    align-items: center; /* 垂直居中 */
    height: 1.5em; /* 设置容器高度 */
  }
  
  .highlight {
    color: #ffffff; /* 设置字体颜色为白色 */
    margin: 0; /* 移除默认的margin */
  }

.timeline {
  list-style: none;
  padding: 0;
  position: relative;
}

.timeline::before {
  content: '';
  position: absolute;
  top: 0;
  bottom: 0;
  left: 30px;
  width: 4px;
  background: #0065bd;
}

.timeline-item {
  padding: 20px 0;
  position: relative;
}

.timeline-marker {
  position: absolute;
  left: 26px;
  width: 12px;
  height: 12px;
  background: #0065bd;
  border-radius: 50%;
}

.timeline-content {
  padding-left: 60px;
}

.boxline {
  list-style: none;
  padding: 0;
  position: relative;
}

.boxline-item {
  position: relative;
  margin-top: 5em;
  margin-bottom: 5em;
}

.boxline-marker {
  position: absolute;
  left: 20px;
  width: 40px;
  height: 40px;
  line-height: 40px;
  text-align: center;
  font-weight: bold;
  color: white;
  background: rgb(48, 191, 248);
  border-radius: 4px;
}

.boxline-content {
  padding-left: 70px;
}

.boxline-content h2 {
  color: black !important;
}

.card-container {
  display: flex;
  justify-content: center;
}

.card {
  background-color: #cceeff;
  border-radius: 5px;
  padding: 20px;
  width: 250px;
  box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
  margin: 20px 30px; /* 上下边距为 20px，左右边距为 10px */
  display: inline-block;
}

.card h2 {
  margin-top: 0;
  margin-bottom: 10px;
}

.card p {
  margin: 0;
}
</style>
![bg](images/cover.png)



---

![bg](./images/content.png)
# Table of Contents

### 1. Motivation
### 2. Introduction
### 3. Framework Design
### 4. Evaluation & Results
### 5. Limitations & Future Work


---

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
                        </div></li></ul>


---

![bg](./images/content.png)
# Motivation
<ul class="timeline">
<li class="timeline-item">
                        <div class="timeline-marker"></div>
                        <div class="timeline-content">
                          <h4>Research trends are important</h4>
                          By researching trends, we can stay ahead of the curve and ensure that our work is always <b>cutting-edge</b>.
                        </div></li><li class="timeline-item">
                        <div class="timeline-marker"></div>
                        <div class="timeline-content">
                          <h4>Challenges in identifying research trends</h4>
                          <ul>
  <li><b>Lack of standardization</b>: Research data is often presented in different formats and with different terminologies, making it difficult to compare and analyze.</li>
  <li><b>Information overload</b>: With the sheer volume of research being produced every day, it can be difficult to know where to start looking for trends.</li>
  <li><b>Noise in the data</b>: Not all research is equally important or reliable, and it can be difficult to filter out the irrelevant or low-quality studies.</li>
  <li><b>Changing landscape</b>: Research trends can shift rapidly in response to new discoveries and technologies, making it difficult to keep up with the latest developments.</li>
</ul>
                        </div></li></ul>


---

![bg](./images/content.png)
# Motivation
<ul class="timeline">
<li class="timeline-item">
                        <div class="timeline-marker"></div>
                        <div class="timeline-content">
                          <h4>Research trends are important</h4>
                          By researching trends, we can stay ahead of the curve and ensure that our work is always <b>cutting-edge</b>.
                        </div></li><li class="timeline-item">
                        <div class="timeline-marker"></div>
                        <div class="timeline-content">
                          <h4>Challenges in identifying research trends</h4>
                          <ul>
  <li><b>Lack of standardization</b>: Research data is often presented in different formats and with different terminologies, making it difficult to compare and analyze.</li>
  <li><b>Information overload</b>: With the sheer volume of research being produced every day, it can be difficult to know where to start looking for trends.</li>
  <li><b>Noise in the data</b>: Not all research is equally important or reliable, and it can be difficult to filter out the irrelevant or low-quality studies.</li>
  <li><b>Changing landscape</b>: Research trends can shift rapidly in response to new discoveries and technologies, making it difficult to keep up with the latest developments.</li>
</ul>
                        </div></li><li class="timeline-item">
                        <div class="timeline-marker"></div>
                        <div class="timeline-content">
                          <h4>The need for an automated framework</h4>
                          Automated literature search and analysis based on <b>machine learning</b> can save time and resources while ensuring accuracy.
                        </div></li></ul>


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
To better understand the the task we are facing, we define the task of **Research Trend Analysis (RTA)** as follows:


**Definition** (Research Trend Analysis)
Consider a collection of literature papers $\mathcal{L} = {L_1, L_2, \ldots, L_n}$. The goal of research trend analysis is to identify $k$ research trends $T_1, T_2, \ldots, T_k$. Each research trend $T_i$ is characterized by a trend text $W_i$, which consists of phrases like "reinforcement learning", and a subset of literature papers $C_i \subseteq \mathcal{L}$ (i.e., a cluster) that belong to this trend.
    


---

![bg](./images/content.png)

# Introduction
To better understand the the task we are facing, we define the task of **Research Trend Analysis (RTA)** as follows:


**Definition** (Research Trend Analysis)
Consider a collection of literature papers $\mathcal{L} = {L_1, L_2, \ldots, L_n}$. The goal of research trend analysis is to identify $k$ research trends $T_1, T_2, \ldots, T_k$. Each research trend $T_i$ is characterized by a trend text $W_i$, which consists of phrases like "reinforcement learning", and a subset of literature papers $C_i \subseteq \mathcal{L}$ (i.e., a cluster) that belong to this trend.

<center>
<img src="./images/intro.png" alt="intro" width=65%>
</center>

        


---

![bg](./images/content.png)
# Research Questions
<ul class="boxline">
<li class="boxline-item">
    <div class="boxline-marker">1</div>
    <div class="boxline-content"><h2>How do we represent papers?</h2></div>
  </li>
<li class="boxline-item">
    <div class="boxline-marker">2</div>
    <div class="boxline-content"><h2>How do we determine the research trends from papers?</h2></div>
  </li>
<li class="boxline-item">
    <div class="boxline-marker">3</div>
    <div class="boxline-content"><h2>How do we evaluate the performance?</h2></div>
  </li>
</ul>



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
# Framework Design - Overview (1)
<div class="card-container">
<div class="card">
    <h2>Text Encoding Module</h2>
    <p>
      <ul><li>Encode paper abstracts into vectors</li><li>Use Transformer-based Encoder models</li><li>Tackle RQ 1</li></ul>
    </p>
  </div>
</div>



---

![bg](./images/content.png)
# Framework Design - Overview (2)
<div class="card-container">
<div class="card">
    <h2>Text Encoding Module</h2>
    <p>
      <ul><li>Encode paper abstracts into vectors</li><li>Use Transformer-based Encoder models</li><li>Tackle RQ 1</li></ul>
    </p>
  </div>
<div class="card">
    <h2>Clustering Module</h2>
    <p>
      <ul><li>Cluster the paper abstracts</li><li>Use ML algorithms such as KMeans</li><li>Papers within the same cluster have similar research trends</li><li>Tackle RQ 2</li></ul>
    </p>
  </div>
</div>



---

![bg](./images/content.png)
# Framework Design - Overview (3)
<div class="card-container">
<div class="card">
    <h2>Text Encoding Module</h2>
    <p>
      <ul><li>Encode paper abstracts into vectors</li><li>Use Transformer-based Encoder models</li><li>Tackle RQ 1</li></ul>
    </p>
  </div>
<div class="card">
    <h2>Clustering Module</h2>
    <p>
      <ul><li>Cluster the paper abstracts</li><li>Use ML algorithms such as KMeans</li><li>Papers within the same cluster have similar research trends</li><li>Tackle RQ 2</li></ul>
    </p>
  </div>
<div class="card">
    <h2>Keyphrase Generator Module</h2>
    <p>
      <ul><li>Generate Research Trends for each cluster</li><li>Use Transformer models</li><li>Tackle RQ 2</li></ul>
    </p>
  </div>
</div>



---

![bg](./images/content.png)

# Framework Design - Pipeline (1)

<center>
<img src="./images/pipeline.png" width = 90%>
</center>
    


---

![bg](./images/content.png)

# Framework Design - Pipeline (2)

<center>
<img src="./images/pipeline.png" width = 90%>
</center>

1. Every paper abstract is transformed into a 768-dimensional vector (embedding)
    


---

![bg](./images/content.png)

# Framework Design - Pipeline (3)

<center>
<img src="./images/pipeline.png" width = 90%>
</center>

1. Every paper abstract is transformed into a 768-dimensional vector (embedding)
2. Embeddings are clustered based on their similarity, measured by distance
    


---

![bg](./images/content.png)

# Framework Design - Pipeline (4)

<center>
<img src="./images/pipeline.png" width = 90%>
</center>

1. Every paper abstract is transformed into a 768-dimensional vector (embedding)
2. Embeddings are clustered based on their similarity, measured by distance
3. For each cluster, research trends are identified, generated, and summarized
   



---

![bg](./images/content.png)

# Framework Design - Text Encoding Module (1)

<center>
<img src="./images/pipeline_textencoder.png" width = 90%>
</center>


- Goal: Transform literature abstracts into vector representations for clustering     



---

![bg](./images/content.png)

# Framework Design - Text Encoding Module (2)

<center>
<img src="./images/pipeline_textencoder.png" width = 90%>
</center>


- Goal: Transform literature abstracts into vector representations for clustering
- Approach: Use transformer-based encoder models due to their exceptional performance
  - Examples of encoder models: BERT, RoBERTa, DistilBERT



---

![bg](./images/content.png)

# Framework Design - Text Encoding Module (3)

<center>
<img src="./images/pipeline_textencoder.png" width = 90%>
</center>


- Goal: Transform literature abstracts into vector representations for clustering
- Approach: Use transformer-based encoder models due to their exceptional performance
  - Examples of encoder models: BERT, RoBERTa, DistilBERT
- Selected model: all-mpnet-base-v2
  - Strong clustering performance
  - Moderate word embedding dimension (768)
  - Lower computational costs



---

![bg](./images/content.png)

# Framework Design - Clustering (1)
<center>
<img src="./images/pipeline_clustering.png" width = 90%>
</center>

---
# Framework Design - Clustering (2)
<center>
<img src="./images/pipeline_clustering.png" width = 90%>
</center>

- Clustering:
  - Groups similar literature abstracts
  - Algorithms used: K-Means, DBSCAN, Agglomerative Clustering, Gaussian Mixture Model (GMM), Spectral Clustering
    - determine or estimate the optimal number of clusters without prior specification


---
# Framework Design - Clustering (3)
<center>
<img src="./images/pipeline_clustering.png" width = 90%>
</center>

- Clustering:
  - Groups similar literature abstracts
  - Algorithms used: K-Means, DBSCAN, Agglomerative Clustering, Gaussian Mixture Model (GMM), Spectral Clustering
    - determine or estimate the optimal number of clusters without prior specification
- Dimensionality Reduction:
  - High-dimensional vectors increase computational complexity and storage space requirements
  - Use PCA (Principal Component Analysis) to reduce dimensionality
    - only assumes normalized input data
    
---

# Framework Design - Keyphrase Generation (1)
<center>
<img src="./images/pipeline_key.png" width = 90%>
</center>

---

# Framework Design - Keyphrase Generation (2)
<center>
<img src="./images/pipeline_key.png" width = 90%>
</center>

- Keyphrase Generator:
  - Uses KeyBART for keyphrase generation
  - State-of-the-art performance on keyphrase generation and other NLP tasks
  - Fine-tuning with **manually annotated RTA dataset (90 samples)**

---

# Framework Design - Keyphrase Generation (3)
<center>
<img src="./images/pipeline_key.png" width = 90%>
</center>

- Keyphrase Generator:
  - Uses KeyBART for keyphrase generation
  - State-of-the-art performance on keyphrase generation and other NLP tasks
  - Fine-tuning with **manually annotated RTA dataset (90 samples)**
- Adapters Technique:
  - Hard to fully fine-tune KeyBART model (560M parameters)
  - Integrates adapters with KeyBART to retain original knowledge
      - Adapter layers added between KeyBART's decoder layers
      - Experiments with hidden dimensions of 32, 64, 128, 256, and 512
  - **"KeyBART-adapter"**
    - 0.8M ~ 12M parameters




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

# Evaluation & Results

We Have done 3 quantitative  experiments and 1 qualitative experiment.

---
# Evaluation & Results - Quantitative Experiments (1)

  1. Clustering Evaluation:
     - Performed on Abstract-Only dataset
     - Metrics: Adjusted Rand Index (ARI), Silhouette Score, Calinski-Harabasz Index (CHI)

---

# Evaluation & Results - Quantitative Experiments (2)

  1. Clustering Evaluation:
     - Performed on Abstract-Only dataset
     - Metrics: Adjusted Rand Index (ARI), Silhouette Score, Calinski-Harabasz Index (CHI)
  2. Ablation study on Dimensionality Reduction:
     - Compare clustering results with original high-dimensional and reduced-dimensional embeddings

---

# Evaluation & Results - Quantitative Experiments (3)

  1. Clustering Evaluation:
     - Performed on Abstract-Only dataset
     - Metrics: Adjusted Rand Index (ARI), Silhouette Score, Calinski-Harabasz Index (CHI)
  2. Ablation study on Dimensionality Reduction:
     - Compare clustering results with original high-dimensional and reduced-dimensional embeddings
  3. Research Trend Generation Evaluation:
     - Train KeyBART-adapter and KeyBART on RTA training set
     - Fine-tune hyperparameters using the validation set and experiment on test set
     - Metrics: F-score@M (harmonic mean of precision and recall for top-M generated keywords)

---
# Evaluation & Results - Quantitative Experiments (4)

## Clustering Evaluation Result

| Algorithm       | Adjusted Rand Index (ARI) | Silhouette Score | Calinski-Harabasz Index (CHI) |
|-----------------|---------------------|------------------|-------------------------|
| KMeans          | 0.6944              | **0.0843**       | **17.362**              |
| GMM             | **0.7202**           | 0.0839           | 17.356                  |
| DBSCAN          | -                   | -                | -                       |
| Agglomerative   | 0.6201              | 0.0782           | 16.261                  |
| Spectral        | 0.7087              | 0.0836           | 17.349                  |

- GMM performed best in Adjusted Rand Index
- KMeans scored highest in Silhouette Score and Calinski-Harabasz Index
- Choosing the best clustering algorithm depends on desired cluster qualities:
  - Higher intra-cluster similarity & Lower inter-cluster similarity (KMeans)
  - Closer alignment with ground truth labeling (GMM)

---
# Evaluation & Results - Quantitative Experiments (5)

## Ablation on Dimensionality Reduction Evaluation Result

| Algorithm        | Adjusted Rand Index (ARI) | Silhouette Score | Calinski-Harabasz Index (CHI) |
|------------------|---------------------|------------------|-------------------------|
| KMeans + PCA     | 0.6944              | 0.09061          | **18.410**              |
| GMM + PCA        | 0.7065              | **0.09064**      | 18.402                  |
| DBSCAN + PCA     | -                   | -                | -                       |
| Agglomerative + PCA | 0.6209          | 0.0841          | 17.212                  |
| Spectral + PCA   | **0.7087**          | 0.0900           | 18.395                  |


- Minimal impact of PCA on ARI
  - even a slight decrease for GMM
- Silhouette Score and CHI improve across all clustering algorithms
- Incorporating PCA may enhance overall clustering quality
  - Better intra-cluster similarity
  - Better inter-cluster dissimilarity


---
# Evaluation & Results - Quantitative Experiments (6)

## Research Trend Generation Evaluation Result

|                   | F-score@M (%) | Precision@M (%) | Recall@M (%) |
|-------------------|---------------|-----------------|--------------|
| KeyBART-adapter   | **33.25**     | **40.33**       | 30.07        |
| KeyBART           | 32.75         | 32.92           | **33.08**    |

KeyBART-adapter performs better in keyphrase generation overall
  - F-score@M and Precision@M are higher for KeyBART-adapter
  - KeyBART has a slightly higher Recall@M



---
# Evaluation & Results - Quantitative Experiments (6)

## Research Trend Generation Evaluation Result

|                   | F-score@M (%) | Precision@M (%) | Recall@M (%) |
|-------------------|---------------|-----------------|--------------|
| KeyBART-adapter   | **33.25**     | **40.33**       | 30.07        |
| KeyBART           | 32.75         | 32.92           | **33.08**    |



**In research trend analysis, precision is often more important than recall**
- Researchers prefer *fewer precise* trends over a larger set of related but less accurate ones
  - helps focus on the most critical developments in a field
- Considering precision, KeyBART-adapter is the more suitable model for research trend analysis.

---
# Evaluation & Results - Qualitative Experiments (1)

Human evaluation with 5 researchers from various domains

## Two steps in the evaluation process

1. Researchers given research trends and clusters generated by TrendFlow framework with two configurations:
    - Configuration 1: GMM clustering (no dimensionality reduction) and KeyBART-adapter for trend generation
    - Configuration 2: Same as Configuration 1 but with KeyBART for trend generation
2. Participants rate relevance, coherence of clusters, and accuracy of generated research trends on a 5-point Likert scale (1 is lowest, 5 is highest)




---

![bg](./images/content.png)
# Evaluation & Results - Qualitative Experiments (2)
<div class="card-container">
<div class="card">
    <h2>Relevance of Clusters</h2>
    <p>
      <ul><li>Are the clusters meaningful or useful for the RTA task?</li></ul>
    </p>
  </div>
<div class="card">
    <h2>Consistency of Clusters</h2>
    <p>
      <ul><li>Are the data points within the same cluster similar to each other?</li></ul>
    </p>
  </div>
<div class="card">
    <h2>Accuracy of Research Trends</h2>
    <p>
      <ul><li>Do the generated research trends represent the actual trends?</li></ul>
    </p>
  </div>
</div>



---

![bg](./images/content.png)

    
# Evaluation & Results - Qualitative Experiments (3)

## Human Evaluation Result
| Configuration | Relevance of Clusters | Coherence of Clusters | Accuracy of Research Trends |
|---------------|-----------------------|-----------------------|-----------------------------|
| Conf1 (KeyBART-adapter)         | 4.66                  | 4.33                  | **4.33**                    |
| Conf2 (KeyBART)        | 4.66                  | 4.33                  | 4.16                        |

- Both configurations effectively cluster research topics
- KeyBART-adapter outperforms KeyBART in generating accurate research trends

---

# Aside: Web App Live Demo

https://huggingface.co/spaces/Adapting/TrendFlow




---

![bg](./images/content.png)
# Table of Contents

### 1. Motivation
### 2. Introduction
### 3. Framework Design
### 4. Evaluation & Results
### <div class ="highlight-wrapper"><div class="highlight-container"><div class="highlight"> 5. Limitations & Future Work</div></div></div>


---

![bg](./images/content.png)
# Limitations & Future Work
<div class="card-container">
<div class="card">
    <h2>Constrained summarization of generated research trends</h2>
    <p>
      <ul><li>TrendFlow generates research trends for each paper within a single cluster, which can result in an overwhelming number of trends.</li><li>Refined post-processing of the generated research trends is necessary.</li><li>Current approach to grouping similar research trends: union-find algorithm.</li><li>Advanced methods (neural network-based) may be necessary to handle larger datasets.</li></ul>
    </p>
  </div>
</div>



---

![bg](./images/content.png)
# Limitations & Future Work
<div class="card-container">
<div class="card">
    <h2>Constrained summarization of generated research trends</h2>
    <p>
      <ul><li>TrendFlow generates research trends for each paper within a single cluster, which can result in an overwhelming number of trends.</li><li>Refined post-processing of the generated research trends is necessary.</li><li>Current approach to grouping similar research trends: union-find algorithm.</li><li>Advanced methods (neural network-based) may be necessary to handle larger datasets.</li></ul>
    </p>
  </div>
<div class="card">
    <h2>Domain-specific adaptations</h2>
    <p>
      <ul><li>The RTA datasets were annotated by only sampling literature in machine learning and deep learning-related domains.</li><li>The TrendFlow framework's generalizability and adaptability to different research domains have not been extensively explored.</li><li>The framework's performance could potentially vary across different domains.</li><li>Further research should investigate whether domain-specific adaptations or customizations are necessary to optimize its performance across various fields of study.</li></ul>
    </p>
  </div>
</div>



---

![bg](./images/content.png)
# Limitations & Future Work
<div class="card-container">
<div class="card">
    <h2>Constrained summarization of generated research trends</h2>
    <p>
      <ul><li>TrendFlow generates research trends for each paper within a single cluster, which can result in an overwhelming number of trends.</li><li>Refined post-processing of the generated research trends is necessary.</li><li>Current approach to grouping similar research trends: union-find algorithm.</li><li>Advanced methods (neural network-based) may be necessary to handle larger datasets.</li></ul>
    </p>
  </div>
<div class="card">
    <h2>Domain-specific adaptations</h2>
    <p>
      <ul><li>The RTA datasets were annotated by only sampling literature in machine learning and deep learning-related domains.</li><li>The TrendFlow framework's generalizability and adaptability to different research domains have not been extensively explored.</li><li>The framework's performance could potentially vary across different domains.</li><li>Further research should investigate whether domain-specific adaptations or customizations are necessary to optimize its performance across various fields of study.</li></ul>
    </p>
  </div>
<div class="card">
    <h2>Scalability</h2>
    <p>
      <ul><li>The TrendFlow framework's scalability and performance with large-scale datasets have not been thoroughly evaluated.</li><li>Increasing volume of research publications could pose challenges related to computational resources, processing time, and memory requirements.</li><li>Future work should consider optimizing the framework's performance and evaluating its scalability with larger datasets.</li></ul>
    </p>
  </div>
</div>



---

![bg](./images/content.png)
<div style="display: flex; justify-content: center; align-items: center; height: 100vh; text-align: center;padding-left=200px">
  <h1 style="margin: 0 auto;">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Thanks for Attention! Any Questions?</h1>
</div>
