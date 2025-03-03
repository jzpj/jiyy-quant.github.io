---
title: "Black-Scholes模型Python实现"
date: 2024-03-10
categories: [期权定价]
---

## 一、模型公式
$$ C = S_0 N(d_1) - K e^{-rT} N(d_2) $$

## 二、Python代码
```python
from scipy.stats import norm
def bs_price(S, K, T, r, sigma):
    d1 = (np.log(S/K) + (r + 0.5*sigma**2)*T)/(sigma*np.sqrt(T))
    # ...完整代码...
