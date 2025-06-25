---
layout: post
title: "Biased Flip Picks [Jane Street]"
date: 2024-12-03
tags: [probability]
---

## 🎲 Is the Coin Double-Headed?

A group includes **98 unbiased (fair) coins**, **1 coin with heads on both sides**, and **1 coin with tails on both sides**.  
A coin is picked at random and tossed once — it lands on **heads**.

> **What is the probability that the tossed coin is the one with two heads?**

---

### 🔍 Step-by-Step Using Bayes' Theorem

Let:

- **D** = event that the coin is the double-headed coin  
- **H** = event that we observe a head on the toss

We are looking for: P(D | H) 

Using **Bayes' Theorem**:

P(D | H) = [P(H | D) × P(D)] / P(H)


---

### 🔢 Calculating Each Term

There are 100 coins in total:

- 98 are fair coins  
- 1 is double-headed  
- 1 is double-tailed

#### 🔹 P(D) = 1/100  
Only one coin is double-headed.

#### 🔹 P(H | D) = 1  
If we choose the double-headed coin, it **always shows heads**.

#### 🔹 P(F) = 98/100  
Probability of choosing a fair coin.

#### 🔹 P(H | F) = 1/2  
Fair coins show heads half the time.

#### 🔹 P(T) = 1/100  
Probability of choosing the double-tailed coin.

#### 🔹 P(H | T) = 0  
The double-tailed coin **can never** show heads.

---

### 🧮 Total Probability of Observing a Head

Now we calculate `P(H)` by considering all three coin types:

P(H) = P(H | D) × P(D) + P(H | F) × P(F) + P(H | T) × P(T)
= 1 × (1/100) + (1/2) × (98/100) + 0 × (1/100)
= 1/100 + 49/100
= 50/100 = 1/2


---

### ✅ Final Calculation

\[
P(D | H) = \frac{1 × \frac{1}{100}}{\frac{1}{2}} = \frac{1}{100} × \frac{2}{1} = \frac{1}{50}
\]

---

### 🎯 Final Answer:

> The probability that the tossed coin was the double-headed one, **given that we observed heads**, is **1⁄50**.



