---
id: T20260529-001
created: 2026-05-29
source:
  - text
related:
  - "[[Maths]]"
  - "[[Maths - Clarifying Concepts]]"
priority:
status:
title: MT - symmetric matrices & choosing eigenvectors
---

Did this Q and asked #gem: [Finding Characteristic Polynomial and Eigenvectors - Google Gemini](https://gemini.google.com/app/179546c57b84e42d?is_sa=1&is_sa=1&android-min-version=301356232&ios-min-version=322.0&campaign_id=bkws&utm_source=sem&utm_medium=paid-media&utm_campaign=bkws&pt=9008&mt=8&ct=p-growth-sem-bkws&gclsrc=aw.ds&gad_source=1&gad_campaignid=20108148187&gbraid=0AAAAApk5Bhkq3nEayagD6fOOAKliOMoL3&gclid=Cj0KCQiAsY3LBhCwARIsAF6O6XiH8OkK2V1WTUmiFFg8e-oJe7g4mNNFMu6WcWaDhBcPsKktHPU2xQ8aAqYfEALw_wcB)
![[Pasted image 20260529092112.png]]
because I didn't understand why in the solutions you have to force the eigenvectors to be orthonormal:
![[Pasted image 20260529092423.png]]

---
Because $A$ is a **symmetric matrix**, the Spectral Theorem guarantees some beautiful properties. However, there is a subtle distinction between what happens _automatically_ and what we have to _force_ by hand when an eigenvalue repeats.

Let's break down exactly why the mark scheme specifies this and how to choose your vectors.

### 1. Why do they need to be orthogonal and of length 1?

The question asks for a matrix $M$ such that:

$$M^T M = I$$

This is the literal definition of an **orthogonal matrix**. For $M^T M$ to equal the identity matrix, the columns of $M$ _must_ form an **orthonormal basis**.

If you compute the matrix multiplication $M^T M$ using columns $\mathbf{v}_1, \mathbf{v}_2, \mathbf{v}_3$, it looks like this:

$$M^T M = \begin{pmatrix} — \mathbf{v}_1^T — \\ — \mathbf{v}_2^T — \\ — \mathbf{v}_3^T — \end{pmatrix} \begin{pmatrix} \mid & \mid & \mid \\ \mathbf{v}_1 & \mathbf{v}_2 & \mathbf{v}_3 \\ \mid & \mid & \mid \end{pmatrix} = \begin{pmatrix} \mathbf{v}_1 \cdot \mathbf{v}_1 & \mathbf{v}_1 \cdot \mathbf{v}_2 & \mathbf{v}_1 \cdot \mathbf{v}_3 \\ \mathbf{v}_2 \cdot \mathbf{v}_1 & \mathbf{v}_2 \cdot \mathbf{v}_2 & \mathbf{v}_2 \cdot \mathbf{v}_3 \\ \mathbf{v}_3 \cdot \mathbf{v}_1 & \mathbf{v}_3 \cdot \mathbf{v}_2 & \mathbf{v}_3 \cdot \mathbf{v}_3 \end{pmatrix}$$

For this result to be the Identity Matrix $\begin{pmatrix} 1 & 0 & 0 \\ 0 & 1 & 0 \\ 0 & 0 & 1 \end{pmatrix}$:

- **The diagonal entries must equal 1:** $\mathbf{v}_i \cdot \mathbf{v}_i = 1 \implies$ Each vector must have a **length (norm) of 1**. Eigenvectors do _not_ naturally have a length of 1; they can be scaled to any length, so we must normalize them manually.
    
- **The off-diagonal entries must equal 0:** $\mathbf{v}_i \cdot \mathbf{v}_j = 0 \implies$ The vectors must be **orthogonal** to each other.
    

### 2. Doesn't orthogonality happen naturally for symmetric matrices?

**Only between distinct eigenspaces.** The theorem states that eigenvectors corresponding to _different_ eigenvalues of a symmetric matrix are automatically orthogonal.

- Therefore, the eigenvector for $\lambda = 3$ is **automatically orthogonal** to any eigenvector you pick for $\lambda = -2$. You don't have to do any work there.
    

**The Trap:** Because $\lambda = -2$ has a **multiplicity of 2**, its eigenspace is a 2D plane. Inside a 2D plane, you can pick infinitely many pairs of vectors to span it, and **they are not automatically orthogonal to each other**. You have to deliberately choose a pair that meets at a $90^\circ$ angle.

### 3. How do you determine which eigenvectors to take?

The solution shows that any eigenvector for $\lambda = -2$ looks like:

$$\mathbf{v} = \begin{pmatrix} -2s \\ s \\ t \end{pmatrix}$$

This vector has two independent free variables ($s$ and $t$), which confirms it's a 2D plane. To find two orthogonal vectors spanning this plane, the easiest trick is to isolate the variables one at a time:

- **Vector 1 (Set $s = 0, t = 1$):**
    
    $$\mathbf{u}_2 = \begin{pmatrix} 0 \\ 0 \\ 1 \end{pmatrix}$$
    
- **Vector 2 (Set $s = 1, t = 0$):**
    
    $$\mathbf{u}_3 = \begin{pmatrix} -2 \\ 1 \\ 0 \end{pmatrix}$$
    

#### Check for Orthogonality:

Let's check their dot product:

$$\mathbf{u}_2 \cdot \mathbf{u}_3 = (0)(-2) + (0)(1) + (1)(0) = 0$$

Because the dot product is exactly 0, our choice of isolating the variables naturally gave us two perpendicular vectors. _(If a random choice doesn't give 0, you would normally have to use the Gram-Schmidt process, but splitting the free variables cleanly usually works perfectly on exam problems like this)._

#### Normalize Them (Make length = 1):

- For $\mathbf{u}_2$: The length is $\sqrt{0^2 + 0^2 + 1^2} = 1$. It’s already normalized!
    
    $$\mathbf{v}_2 = \begin{pmatrix} 0 \\ 0 \\ 1 \end{pmatrix}$$
    
- For $\mathbf{u}_3$: The length is $\sqrt{(-2)^2 + 1^2 + 0^2} = \sqrt{5}$. Divide by $\sqrt{5}$:
    
    $$\mathbf{v}_3 = \frac{1}{\sqrt{5}}\begin{pmatrix} -2 \\ 1 \\ 0 \end{pmatrix}$$
    

Combine these with your normalized vector from $\lambda = 3$, and you have the columns for your matrix $M$.


---
*Created: 2026-05-29 09:20*