---
id: T20260527-002
created: 2026-05-27
source:
  - text
related:
  - "[[Maths]]"
priority:
status:
title: MT - choosing a trig sub
---

from #gem

## 3. How to Choose a Substitution in General

When you see a radical of the form $\sqrt{a^2 + b^2x^2}$, $\sqrt{a^2 - b^2x^2}$, or $\sqrt{b^2x^2 - a^2}$, you have a direct choice between standard circular trig and hyperbolic trig.

Here is a quick reference table to guide your intuition:

|**Form in Integral**|**Standard Trig Substitution**|**Hyperbolic Substitution**|**Why Choose Hyperbolic?**|
|---|---|---|---|
|**$\sqrt{a^2 + x^2}$**|$x = a\tan(u)$|$x = a\sinh(\theta)$|**Highly Recommended.** Avoids the messy $\sec^3(u)$ integral; integrates smoothly using basic exponents/double-angle identities.|
|**$\sqrt{x^2 - a^2}$**|$x = a\sec(u)$|$x = a\cosh(\theta)$|**Good alternative.** Avoids $\sec(u)\tan^2(u)$ combinations.|
|**$\sqrt{a^2 - x^2}$**|$x = a\sin(u)$|$x = a\tanh(\theta)$|**Stick to standard $\sin(u)$.** Circular trig handles this beautifully because $\cos^2(u) = 1 - \sin^2(u)$ is incredibly clean. Hyperbolic substitution here often gets messy.|

### Summary Checklist for Integrals

1. If you see $\sqrt{a^2 - x^2}$, default to **circular trig** ($x = a\sin(u)$).
    
2. If you see $\sqrt{a^2 + x^2}$ or $\sqrt{x^2 - a^2}$ and you want to bypass integration by parts or tricky secant/tangent reductions, lean toward **hyperbolic functions**.
    
3. If you aren't comfortable converting inverse hyperbolic functions back to regular logarithms at the evaluation step, stick with your **tangent substitution**—it is reliable and always gets you over the finish line if you know your secant integrals!
    

Did the evaluation of the definite integral limits yield the same final result for you, or would you like to walk through the boundary conversion step for either substitution method?


---
*Created: 2026-05-27 11:20*