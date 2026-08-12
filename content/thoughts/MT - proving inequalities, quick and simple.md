---
id: T20260604-001
created: 2026-06-04
source:
  - text
related:
  - "[[Maths]]"
priority:
status:
title: MT - proving inequalities, quick and simple
---
from [[S-001]], [[Thu 04-06-2026]]

![[Pasted image 20260604084125.png]]

**Proving log(n) < n**

Since the solution sheet explicitly challenges you to **"(prove the first inequality!)"**, here is a quick, rigorous way to show that $\log(n) < n$ for all $n \geq 2$ (or even all $n > 0$ if using real numbers $x$).

Let's define a function $f(x) = x - \log(x)$ for $x \geq 2$. We want to show that $f(x) > 0$.

1. **Check the boundary:** For $x = 2$, $f(2) = 2 - \log(2) \approx 1.307 > 0$.
    
2. **Check the derivative to see the trend:**
    
    $$f'(x) = 1 - \frac{1}{x}$$
    
3. **Analyze the growth:** For all $x \geq 2$, the term $\frac{1}{x} \leq \frac{1}{2}$, which means $f'(x) \geq \frac{1}{2} > 0$.
    

Because the derivative is strictly positive, the gap between $x$ and $\log(x)$ is strictly growing larger as $x$ increases. Since it started out positive at $x=2$ and only grows from there, $\log(n)$ is guaranteed to be less than $n$ for all $n \geq 2$.


---
*Created: 2026-06-04 08:41*