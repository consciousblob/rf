---
id: T20260624-003
created: 2026-06-24
source:
  - text
related:
priority: 
status: 
title: "MT - Index Notation"
---

# Raising/Lowering

### Example 1: Raising the First Index

Suppose you have a tensor where both indices are downstairs, $M_{\alpha\beta}$. You want to raise the **first** index ($\alpha$) so that it becomes an upstairs index ($\mu$).

To do this, you multiply by a superscript metric $\eta$ whose second slot contracts with the first slot of $M$:

$$M^\mu_{\ \ \beta} = \eta^{\mu\sigma} M_{\sigma\beta}$$

- **Why it works:** The dummy index $\sigma$ appears exactly once upstairs (on $\eta$) and once downstairs (in the _first_ slot of $M$). They contract and disappear. The first slot of $M$ is pulled upstairs, inheriting the free index $\mu$ from the metric. The second index $\beta$ is left completely untouched.
    

### Example 2: Raising the Second Index

Now suppose you start with that same tensor $M_{\alpha\beta}$, but this time you want to raise the **second** index ($\beta$) so it becomes an upstairs index ($\nu$).

You multiply by a superscript metric $\eta$ whose second slot contracts with the second slot of $M$:

$$M_\alpha^{\ \ \nu} = \eta^{\nu\sigma} M_{\alpha\sigma}$$

- **Why it works:** The dummy index $\sigma$ contracts across the _second_ slot of $M$. The second slot is pulled upstairs, inheriting the free index $\nu$ from the metric. The first index $\alpha$ stays exactly where it was downstairs.
    

### Example 3: Raising Both Indices at Once

If you want to pull _both_ downstairs slots of $M_{\alpha\beta}$ upstairs to become $M^{\mu\nu}$, you need to bring in two separate metric factories—one for each slot. You must use a different dummy letter for each contraction so the algebra doesn't get confused:

$$M^{\mu\nu} = \eta^{\mu\rho} \eta^{\nu\sigma} M_{\rho\sigma}$$

- **Why it works:** * $\eta^{\mu\rho}$ targets the first slot by contracting with $\rho$.
    
    - $\eta^{\nu\sigma}$ targets the second slot by contracting with $\sigma$.
        
    - Both dummy letters ($\rho$ and $\sigma$) are burned up in the summation, leaving behind the clean upstairs indices $\mu$ and $\nu$ in their respective horizontal positions.
        

### Example 4: Lowering an Index

The grammar works exactly the same way in reverse using the downstairs metric $\eta_{\mu\nu}$. Suppose you start with a tensor that has both indices upstairs, $M^{\alpha\beta}$, and you want to lower the second index ($\beta$) to become a downstairs index ($\nu$):

$$M^\alpha_{\ \ \nu} = \eta_{\nu\sigma} M^{\alpha\sigma}$$

- **Why it works:** The dummy index $\sigma$ is upstairs in the second slot of $M$ and downstairs in the second slot of $\eta$. They contract, and the second slot is pulled downstairs, inheriting the free index $\nu$.
    

### Summary Rule for Your Scratchpad

Whenever you write a raising or lowering equation:

1. Identify which horizontal slot you want to change (1st or 2nd).
    
2. Put a temporary dummy letter (like $\sigma$) in that slot on your target tensor.
    
3. Match that dummy letter on a metric tensor ($\eta$), placing it vertically opposite.
    
4. Give the metric your final desired free index (like $\mu$ or $\nu$) in the remaining slot.


---
*Created: 2026-06-24 20:59*