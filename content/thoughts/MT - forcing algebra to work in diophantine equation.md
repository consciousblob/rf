---
id: T20260605-007
created: 2026-06-05
source:
  - text
related:
  - "[[Maths]]"
priority:
status:
title: MT - forcing algebra to work in diophantine equation
---


Working from this question/solution:
![[Pasted image 20260605205939.png]]
(has typo/mistake - see gem below)

From [Solving Linear Diophantine Equations - Google Gemini](https://gemini.google.com/app/12e3ed35c4e1753d?is_sa=1&is_sa=1&android-min-version=301356232&ios-min-version=322.0&campaign_id=bkws&utm_source=sem&utm_medium=paid-media&utm_campaign=bkws&pt=9008&mt=8&ct=p-growth-sem-bkws&gclsrc=aw.ds&gad_source=1&gad_campaignid=20108148187&gbraid=0AAAAApk5Bhkq3nEayagD6fOOAKliOMoL3&gclid=Cj0KCQiAsY3LBhCwARIsAF6O6XiH8OkK2V1WTUmiFFg8e-oJe7g4mNNFMu6WcWaDhBcPsKktHPU2xQ8aAqYfEALw_wcB):

It is completely understandable to look at choices like $m = -\epsilon a$ and $n = \epsilon$ and think, _"How on earth was I supposed to just guess that?"_ The secret is that **mathematicians don't guess these values either.** They work backward using a scratch-pad technique called **undetermined coefficients**, or they use a systematic tool called the **Extended Euclidean Algorithm**.

Here is exactly how you can find those values of $m$ and $n$ on your own in an exam, completely from scratch, using two different methods.

## Method 1: The "Scratch-Pad" Method (Working Backward)

Instead of trying to guess $m$ and $n$ in your head, leave them as blank targets and force the algebra to tell you what they have to be.

### Step 1: Set up the goal

You know your equation is:

$$6m + kn = 1$$

And you have already established that $k = 6a + \epsilon$ (where $\epsilon = \pm 1$). Substitute that $k$ into your equation:

$$6m + (6a + \epsilon)n = 1$$

### Step 2: Expand and group by the parts you can control

Expand the brackets:

$$6m + 6an + \epsilon n = 1$$

Now, look at the terms that have a $6$ in them. Group them together:

$$6(m + an) + \epsilon n = 1$$

### Step 3: Eliminate the clutter

Look at that equation. You want the left side to equal $1$.

The easiest way to make a complicated algebraic expression equal $1$ is to make the heavy, messy part completely disappear ($= 0$) and make the remaining simple part equal $1$.

To make the first part disappear, we set:

$$m + an = 0 \implies m = -an$$

To make the second part equal $1$, we look at what's left:

$$\epsilon n = 1$$

### Step 4: Solve for your targets

Since $\epsilon = \pm 1$, we can multiply both sides by $\epsilon$ (remembering that $\epsilon^2 = 1$):

$$\epsilon^2 n = \epsilon \implies n = \epsilon$$

Now plug $n = \epsilon$ back into your equation for $m$:

$$m = -a(\epsilon) \implies m = -\epsilon a$$

**Boom.** You didn't guess anything. You just forced the algebraic terms you wanted to get rid of to equal $0$.

---
*Created: 2026-06-05 20:58*