---
id: T20260528-001
created: 2026-05-28
source:
  - text
related:
  - "[[Maths]]"
priority:
status:
title: MT - periodic functions & their integrals
---

[Evaluating Periodic Function Integral - Google Gemini](https://gemini.google.com/app/3f9b9a1f1e356f0d?is_sa=1&is_sa=1&android-min-version=301356232&ios-min-version=322.0&campaign_id=bkws&utm_source=sem&utm_medium=paid-media&utm_campaign=bkws&pt=9008&mt=8&ct=p-growth-sem-bkws&gclsrc=aw.ds&gad_source=1&gad_campaignid=20108148187&gbraid=0AAAAApk5Bhkq3nEayagD6fOOAKliOMoL3&gclid=Cj0KCQiAsY3LBhCwARIsAF6O6XiH8OkK2V1WTUmiFFg8e-oJe7g4mNNFMu6WcWaDhBcPsKktHPU2xQ8aAqYfEALw_wcB)
response to 
![[Pasted image 20260528121018.png]]

#gem:
Here is the step-by-step solution to the problem in the image.

### 1. Identify the Key Properties

- **Periodicity:** We are given that $f(x + 1) = f(x)$ for all $x \in \mathbb{R}$. This means $f(x)$ is a periodic function with a period of $T = 1$.
    
- **Integral over one period:** We are given that the integral over the interval $[0, 1]$ (which has a length of 1) is:
    
    $$\int_{0}^{1} f(x) \, dx = 1$$
    

### 2. Properties of Periodic Functions

For any periodic function with period $T$:

1. The integral over any interval of length $T$ is always the same, regardless of where the interval starts:
    
    $$\int_{a}^{a+T} f(x) \, dx = \int_{0}^{T} f(x) \, dx$$
    
2. By extension, the integral over an interval whose length is an integer multiple of the period, say $n \cdot T$, is simply $n$ times the integral over a single period:
    
    $$\int_{a}^{a+nT} f(x) \, dx = n \int_{0}^{T} f(x) \, dx$$
    

### 3. Apply to the Problem

We need to evaluate the integral:

$$\int_{\pi}^{\pi + 3} f(x) \, dx$$

Let's look at the limits of integration:

- **Lower limit:** $a = \pi$
    
- **Upper limit:** $b = \pi + 3$
    
- **Length of the interval:** $(\pi + 3) - \pi = 3$
    

Since the period of our function is $T = 1$, the length of this interval is exactly $3$ full periods ($3 \cdot T = 3$).

Using the property stated above:

$$\int_{\pi}^{\pi + 3} f(x) \, dx = 3 \int_{0}^{1} f(x) \, dx$$

Substitute the given value $\int_{0}^{1} f(x) \, dx = 1$:

$$3 \cdot (1) = 3$$

### Conclusion

The correct option is **B. 3**.


---
*Created: 2026-05-28 12:09*