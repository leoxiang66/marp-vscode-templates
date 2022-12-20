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

## Day 1
### Transformer

---

# Outline

- Intro to  Transformer
- Attention Mechanism in Transformer
- Quadratic Complexity of Attention
 

---

# Outline

- **Intro to  Transformer**
- Attention Mechanism in Transformer
- Quadratic Complexity of Attention

---
# Intro to Transformer
Transformer is a cutting-edge *seqquence-to-sequence* model in NLP.



---
# Intro to Transformer
Transformer is a cutting-edge *seqquence-to-sequence* model in NLP.

<br>
<br>
<br>

<center>
<img src = "https://i.imgur.com/OgjFxGJ.png" alt="seq2seq" width=100%></img>
</center>

---
# Intro to Transformer - Example


<center>
<br>
<br>
<h4>Machine Translation</h4>
<br>
<img src="https://i.imgur.com/Y0QvFEa.png" width=100%></img>
</center>

---
# Intro to Transformer - QA

<br>
<br><br>
<center>
<h1>Any  Questions  So Far?</h1>
</center>


---

# Outline

- Intro to  Transformer
- **Attention Mechanism in Transformer**
- Quadratic Complexity of Attention

---
# Attention Mechanism in Transformer
The core idea of Transformer models is the well-known *Attention*  mechanism.

---

# Attention Mechanism in Transformer
The core idea of Transformer models is the well-known *Attention*  mechanism.
<br>
<center>
<img src = "https://i.imgur.com/ugWYf5L.png" width = 90%>
</center>


--- 
# Attention Mechanism in Transformer
The core idea of Transformer models is the well-known *Attention*  mechanism.
<br>
<center>
<img src = "https://i.imgur.com/ulX4vha.png" width = 90%>
</center>

--- 
# Attention Mechanism in Transformer
The core idea of Transformer models is the well-known *Attention*  mechanism.
<br>
<center>
<img src = "https://i.imgur.com/GGQb6il.png" width = 90%>
</center>

--- 
# Attention Mechanism in Transformer
The core idea of Transformer models is the well-known *Attention*  mechanism.
<br>
<center>
<img src = "https://i.imgur.com/l7eHErw.png" width = 90%>
</center>


--- 
# Attention Mechanism in Transformer
<br>
<br>
<br>
<center>
<h2> How is This Achieved?
</center>


--- 
# Attention Mechanism in Transformer

<br>
<center>
<img src ="https://i.imgur.com/aKLNs1G.png">

**Every vector/embedding  is of dimenstion $D$**
</center>



--- 
# Attention Mechanism in Transformer

<br>
<center>
<img src ="https://i.imgur.com/aKLNs1G.png">
</center>

1. $\forall i \in \{1,2,3\}:\ a_i = \langle q_1, k_1 \rangle$ 
    - the larger $a_i$ is, the more attention is paid


--- 
# Attention Mechanism in Transformer

<br>
<center>
<img src ="https://i.imgur.com/aKLNs1G.png">
</center>

1. $\forall i \in \{1,2,3\}:\ a_i = \langle q_1, k_1 \rangle$ 
2. $a_i$ is normalized s.t. $\sum_i^N a_i = 1$ (By Softmax)


--- 
# Attention Mechanism in Transformer

<br>
<center>
<img src ="https://i.imgur.com/aKLNs1G.png">
</center>

1. $\forall i \in \{1,2,3\}:\ a_i = \langle q_1, k_1 \rangle$ 
2. $a_i$ is normalized s.t. $\sum_i^N a_i = 1$ (By Softmax)
3. $\text{Attention}\left(q_1\right) = \sum_i^Na_i *  v_i$

--- 
# Attention Mechanism in Transformer

<br>
<center>
<img src ="https://i.imgur.com/aKLNs1G.png">



**In this case, the NN will learn to make $a_3$ dominate**
</center>


--- 
# Aside: Softmax

<br>
<br>
<br>

$$
\sigma(\mathbf{z})_i=\frac{e^{z_i}}{\sum_{j=1}^K e^{z_j}} \text { for } i=1, \ldots, K \text { and } \mathbf{z}=\left(z_1, \ldots, z_K\right) \in \mathbb{R}^K
$$

--- 
# Aside: Softmax - Consequence

<center>

<h3 style="color:grey">"Softmax function is proposed as a differentiable generalization of the "winner-take-all" picking maximum operation"</h3>
<br>
<h3 style="color:skyblue">"The large one will become larger and donimate" </h3>

<br>

<h3  style= "color:red">"Competition Mechanism"</h3>

</center>

--- 
# Aside: Softmax - Example

<center>
<img src ="https://i.imgur.com/WhjKHDh.png" width=100%>
<font color="gray" size=3px>Bridle et al. Training stochastic model recognition algorithms as networks can lead to maximum mutual information estimation of parameters. NeurIPS 1989.</font>
</center>


---
# Attention Mechanism - QA

<br>
<br><br>
<center>
<h1>Any  Questions  So Far?</h1>
</center>

---

# Outline

- Intro to  Transformer
- Attention Mechanism in Transformer
- **Quadratic Complexity of Attention**

---

# Quadratic Complexity of Attention
One big limitation of dense (self-) attention is that the computation is $O(N^2)$, where $N$ is the sequence length.


---

# Quadratic Complexity of Attention
One big limitation of dense (self-) attention is that the computation is $O(N^2)$, where $N$ is the sequence length.

<center>
<br>
<img src="https://i.imgur.com/TwRJHiV.png"> 
</center>

---

# Quadratic Complexity of Attention
<center>
<img src="https://i.imgur.com/TwRJHiV.png"> 
</center>

$$
\text{Attention}(Q,K,V)=\ \text{Softmax}(Q K^T)\cdot V
$$
- $Q, K, V \in R^{N\times D}$
    - In our example: $N = 3$ 
- Time Complexity: $O(N^2D)$
- Space Complexity: $O(N^2)$


---
<br>
<br>
<br>
<center>
<h1>Thanks for Attention!

Any Questions?</h1>
</center>




