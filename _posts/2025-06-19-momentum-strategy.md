---
layout: post
title: "Momentum Strategy in Crypto Markets"
date: 2025-06-19
tags: [trading]
---

<div style="text-align: center;">
  <h1>Momentum Strategy in Crypto Markets</h1>
</div>

Momentum strategies are based on a simple but powerful idea:  
**assets that have recently gone up will likely keep going up**, and those that are falling may continue to drop.
People chase performance. When they see Bitcoin rising, they don’t want to miss out.
So they jump in late — and push the price even higher.

🚀 Momentum is part psychology — fear of missing out (FOMO).
---

## 📈 Core Idea

Buy assets with upward price momentum,  
Sell either when the price has risen enough (take profit) or when momentum fades (stop loss) but try to cut that loss quickly.

---

## 🔄 Example
You bought Bitcoin at ₹100 because 5 minutes ago it was ₹90. It was rising.

Now what?

💰 Case 1: It rises to ₹110
You say: "I made 10% profit — let’s sell." ✅
You profit ₹10.

⚠️ Case 2: It starts falling to ₹97
You say: "The momentum is gone — I should sell and cut my loss." ❌
You lose ₹3, but avoid worse losses.

---

## 🧠 Why It Works

- Traders tend to **chase performance**.
- Price movements often reflect **lagged information absorption**.
- Momentum persists more in **volatile, speculative assets**, like crypto.

---

## 🐍 Python Example

Here’s a basic momentum signal using 5-period lookback:

if price[t] > price[t - 5]:
    buy()
else:
    sell()
