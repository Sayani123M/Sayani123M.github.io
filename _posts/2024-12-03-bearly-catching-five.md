---
layout: post
title: "Bearly Catching Five"
date: 2024-12-03
tags: [probability]
---

## 🐟 What's the Chance the 5th Fish Is Caught?

A bear is trying to catch **3 fish** from a stream. It stops fishing once it catches 3. The probability of catching a fish on any given attempt is **1/2**, and each attempt is independent.

We are interested in the following:

> **What is the probability that the bear catches the 5th fish it attempts?**

This means: What’s the probability that the 5th fishing attempt results in a successful catch — *regardless* of how many fish the bear has caught before?

---

### 🔍 Step-by-Step Breakdown Using the Law of Total Probability

Let:

- **C** be the event that the **5th attempt results in a catch**.
- **F** be the event that the bear is still fishing on the 5th attempt (i.e., it has caught fewer than 3 fish in the first 4 attempts).

We apply the **Law of Total Probability**:

P(C) = P(C | F) × P(F) + P(C | Fᶜ) × P(Fᶜ)


#### 🔹 1. `P(C | F) = 1/2`

If the bear is still fishing on the 5th attempt, it tries — and succeeds with probability 1/2.

#### 🔹 2. `P(F)` = probability that the bear has caught **fewer than 3** fish in the first 4 attempts

This is the sum of the probabilities of catching 0, 1, or 2 fish in 4 tries:

P(F) = [C(4, 0) + C(4, 1) + C(4, 2)] × (1/2)^4
= (1 + 4 + 6) × 1/16
= 11/16


#### 🔹 3. `P(C | Fᶜ) = 0`

If the bear has already caught 3 fish in the first 4 attempts, it stops fishing and does not make a 5th attempt. So the probability of catching the 5th fish is 0 in this case.

---

### 🧮 Final Computation

P(C) = (1/2 × 11/16) + (0 × 5/16) = 11⁄32


---

### ✅ Final Answer:

> The probability that the 5th fish is caught — regardless of whether it's the 1st, 2nd, or 3rd fish caught — is **11⁄32**.
