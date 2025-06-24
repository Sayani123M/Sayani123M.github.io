---
layout: post
title: "Monty Hall Problem"
date: 2025-06-24
---
<div style="text-align: center;">
  <h1>The Monty Hall Problem</h1>
</div>
Imagine you're on a game show. There are **three doors**:

- Behind one is a **brand-new car** 🚗  
- Behind the other two are **goats** 🐐🐐  

You’re asked to pick one door. After your choice, the host—**Monty**, who knows what’s behind every door—opens another door, revealing a goat. He then offers you a choice:  
**Stick with your original door, or switch to the remaining unopened door.**

---

## ❓ Should You Switch?

Yes, **you should always switch**.  
Despite seeming like a 50–50 choice, switching gives you a **2/3 chance** of winning, while staying gives only **1/3**.

---

## 📊 Understanding the Probabilities

When you first choose:
- There’s a **1/3** chance the car is behind your chosen door.
- There’s a **2/3** chance it’s behind one of the other two doors.

Monty opens a door with a goat—he’ll **never open the door with the car**.  
So the **2/3 probability collapses onto the one unopened door** you didn’t pick.

Thus:
- **Staying = 1/3 chance** of winning  
- **Switching = 2/3 chance** of winning ✅

---

## 🧠 Applying Bayes’ Theorem

Let’s dig deeper using **Bayesian reasoning**.

Let:
- A1: Car is behind your original pick  
- A2: Car is behind the other unopened door  
- M: Monty opens a goat door (e.g., Door 3)

We want:  P(A2 | M)

Using Bayes’ Theorem:
    P(A2 | M) = P(M | A2) . P(A2) / P(M)

If:
- P(A1) = P(A2) = 1/3 
- P(M | A2) = 1  (Monty must open Door 3 if car is behind Door 2)
- P(M) accounts for all possible cases=1/3(0.5)+1/3(1)+1/3(1)=5/6

Ultimately, this yields:
    P(A2 | M) = 1 . 1/3 / 5/6 = 2/5

---

## 🎯 Conclusion

What seems like a 50–50 gamble is actually **rigged by information**.  
Monty's action gives you extra insight—if you use it.

**Switching doors doubles your odds of winning.**  
The Monty Hall problem is a classic case of why intuitive reasoning often fails where **probabilistic thinking** prevails.

---

Stay tuned for a future post where we simulate the Monty Hall game using Python!
