---
title:
type:
created: 2026-07-20
modified: 2026-07-20
publish: false
tags:
description: ""
aliases:
  - Electromagnetism, Relativity, QM, QFT, QED
---
Main current areas involved: **Electromagnetism, Relativity, QM, QFT, QED**.

This exploration is something to do with how we move from a classical to quantum regime in physics, particularly applied to electromagnetism, involving:
- Classical electrodynamics (ED), quantum mechanics (QM), quantum field theory (QFT), special relativity (SR), quantum electrodynamics (QED)
- and whatever seems relevant and piques interest as I go along.

---

**Terms:**
- ED = (classical) electromagnetism/electrodynamics
- QED = quantum electrodynamics
- QM = quantum mechanics
- SR = special relativity
- QFT = quantum field theory
---
ACU = "as currently understood"
ACC = "as currently conceived"
Probably mean same thing (used interchangeably), but might have distinct roles in future as I use them and figure out what works/fits.

---


# Blobs
- current
	- Noether's theorem, section 1.3.1, not just electric current/charge
	- current = 4-vector whose divergence vanishes, encoding a locally conserved quantity
- The Hamiltonian (p. 24 Tong)
	- where it comes from, Hamiltonian density - this Hamiltonian is the energy of the free Klein-Gordon field
- Verify the commutators (Tong p. 29)
- Fourier transforms
	- Tong p. 22 (2.5)


# Log

==Next==
- Feynman propagator
- what is a contour?

[[Fri 07-08-2026]]
- Finish notes
- Start poster
- Email Abhinove

Covered:
- Heisenberg picture
- Accounting for causality
	- Defining propagator, ensuring this preserves causality (is 0 for spacelike separation)
- Contours & Feynman Propagator



[[Tue 04-08-2026]]
Klein-Gordon equation.


# To Investigate
Slightly specific stuff I want to look into at some point.

- Show that Maxwell's Lagrangian is Lorentz invariant
- functionals
- why is it "generalised coordinates" and "conjugate momenta"?
- Where do the EoM come from?
	- And where do Hamiltonian equations come from?
- derive Euler-Lagrange from least action derivative
	- p. 15 QFT
- What is a dispersion relation?
- What is a "mode expansion"?
- **Annihilation vs destruction**
- Why is it called "canonical" quantisation?
- What does Klein-Gordan equation do/represent/show? 
- Electromagnetism (EM) vs electrodynamics (ED)
	- I want to tease the terms apart - ACU, EM represents the general phenomena of electric/magnetic waves and their "behaviour", while ED refers to a subset of this phenomena, where movement is involved, as contrasted with e.g. electrostatics (static objects, no movement).
	- But for this exploration, I like using ED because of its direct mapping to QED. Like, would it make sense to speak of "quantum electromagnetism"?

# To Practice
- Functional differentiation
- Fourier transforms

# Objects
Objects of interest.

- Hilbert space
- Fock space
- Lagrangian & Hamiltonian
	- Hamilton's principle of least action
	- Kinetic & potential energy
- Index notation
	- Einstein summation convention
- Functionals
- Dirac delta function
- Schrodinger's equation
- Heisenberg uncertainty
- Heisenberg vs Schrodginger picture
- Position & momentum
- Operators
- Hermitian matrices
- Dispersion relation
- Simple harmonic oscillator
- Number operator
- Raising-lowering / creation-annihilation operators
- Vacuum state
- Occupation number representation
- Covariant derivative
- Fields
	- Massless scalar field
- Klein-Gordon equation
- interaction between electron field and electromagnetic field
- real vs virtual photons
- probabilities vs probability amplitudes

# Diverge
[[Physics]]
[[S-002]]

Anything I don't yet know where to put / what to do with.

**Statements I want to fully understand at some point:**
- "Field operators are formed from mode expansions with amplitudes made of creation and annihilation operators."
- "each mass is strongly coupled to its neighbour by the springs" p. 25 QFT
	- strongly coupled?
- p. 25 QFT ~"the excitations in this coupled problem behave exactly like independent oscillators, because we can Fourier transform the problem so that while the masses are coupled in real space, the excitations are uncoupled in reciprocal space"
- Copilot ~"each normal mode oscillates independently and the Fourier transform diagonalises the Hamiltonian into these modes"
- it is the derivative terms, not the potential terms, in the action that contribute to the current (p. 19 Tong)
- Tong p. 31
	- "Recall that in quantum mechanics the position and momentum eigenstates are not good elements of the Hilbert space since they are not normalizable (they normalize to delta-functions). Similarly, in quantum field theory neither the operators φ(~x ), nor a~p are good operators acting on the Fock space. This is because they don’t produce normalizable states."
	- "They are operator valued distributions, rather than functions"






**What motivated the development of QED?**
Classical EM is naturally relativistic (because dealing with light, which moves at the speed of light...) but doesn't account for phenomena occurring at the quantum? (Planck?) scale. Effectively, since EM is a deterministic theory (approach?), like Newtonian mechanics, it can't be used to describe phenomena at the quantum scale, which are *probabilistic.* At what point does EM break down, fail to describe things? I.e., at what point does the universe appear to switch from deterministic to probabilistic (where is the border between macro/micro)? I think this has something to do with the de Broglie wavelength and Compton wavelength: below the de Broglie wavelength, the "wavey" nature of "particles" becomes apparent, and below the Compton wavelength, the "particle" nature of "waves" breaks down - it becomes no longer meaningful to treat objects as particles, and we transition purely into the language of fields (QFT).

QM is non-relativistic - it doesn't account for phenomena occurring near the speed of light, such as the possibility of particle creation or annihilation; that is, QM doesn't account for the number of particles in a (system/interaction?) changing.


---

General solution to Klein-Gordon equation:
![[Pasted image 20260721120059.png|375]]

Below, sometimes "quotes" are used to represent something that might be typically said, to represent typical lingo and its usage in these areas.

- **Fock space**
	- Fock space is the sum of all n-particle Hilbert spaces.
	- "creation/destruction of particles moves between n-particle sectors of Fock space"
- **Infinities**
	- Infra-red (infinite space) vs ultra-violet (high frequency / short distance) divergence
- **Normal modes, k-modes**
	- A k-mode (or normal mode) is a lattice vibration with wavevector k.
- **Quantisation: 1st and 2nd**
	- 1: particles -> waves
	- 2: waves -> particles
	- For 2, consider universe as bundle of simple harmonic oscillators
- **Creation/Annihilation, Raising/Lowering** QFT C2
	- Where do these operators come from?
	- Start with the Hamiltonian for a simple harmonic oscillator, but with the operator versions of p and x.
	- Then, it looks factorisable (if complex i is introduced). But when written in this form, since p and x are not just quantities but are operators, they don't commute (why? what's the commutator for them?)
	- ![[Pasted image 20260722221434.png]]
	- In fact, there is an additional factor (something like 1/2hw), which represents the zero-point energy ? or some kind of ground energy state. but does this somehow cancel when the operators operate? idk
	- Anyway, even though factorising doesn't give back exactly the same hamiltonian, the resulting factors are useful enough to extract as objects in their own right - these are the raising/lowering or creation/annihilation operators
	- Raising/lowering: they can add or subtract quanta
	- Creation/annihilation: they can create/destroy quanta ("packets" of energy, which can be thought of as particles ? and this is the nature of the 2nd quantisation, where we show that waves can be thought of as particles)
	- We define the **vacuum state** as the state in which all the harmonic oscillators in the system are at (ground energy state / zero-point energy ?) - that is, if the annihilation operator operates on the vacuum state, it yields 0 (no more destruction/annihilation possible, on bottom rung of ladder)
	- **Occupation number representation** is a way to represent a general state, denoted by a number for the number of quanta in each oscillator - so, each oscillator is represented by a number, which itself represents the number of quanta (contained, held, stored ?) within that oscillator:
		- ![[Pasted image 20260723104622.png]]
		- It is defined as being created by the application/operation ? of the creation operator for that particular oscillator (denoted by the number subscript) n_k times where k is the oscillator, and n is the number of quanta for that oscillator. This is applied to the vacuum to yield the state in which all those oscillators have the specified number of quanta.
- **Electromagnetism**
	- "Electromagnetism" is an umbrella term for the phenomena associated with electric and magnetic waves, which could be thought of as 2 sides of the same coin - one cannot exist without the other.
- **Maxwell's equations, Lorentz force, special relativity**
	- Maxwell's equations relate electric and magnetic fields, describe their relationship, how they interact. Part of this relationship is the fact that a moving electric field induces a magnetic field, and a moving magnetic field induces an electric field. There's something to do with the induced fields being "circulating", which I think means literally circles around the "source" of the inducing field. Is it even accurate to say "moving electric field" in place of the probably more commonly used phraseology of "moving charge"? I would think so, because doesn't a charge create (instate? come along with?) an electric field, and so a moving charge is effectively just a moving electric field?
	- But actually, the fact that e.g. moving E-field induces moving M-field can be derived using simply Coulomb's law (for stationary charge, electrostatics?) plus special relativity. If you imagine a wire with equal number of positive and negative charges, moving in opposite directions (same velocity), by Maxwell's equations (classical EM), there will be a circulating magnetic field around this wire (because the fact there are charges moving represents a current?), and so a charge outside the wire moving at some velocity u (same or different to the charges inside) would experience a magnetic force (Lorentz force?) - or more precisely, a force from this apparent magnetic field. But if we take the perspective of the moving outsider charge (let's call P), and Lorentz transform to its reference frame, then the positive and negative charges inside the wire will have different velocities relative to this outside charge. So, from P's perspective, the wire is in fact charged (whereas from the original "laboratory" frame, the wire is neutral), and so P would, from its perspective, experience an electric force (Coulomb's law). But from the non-P perspective, this force is magnetic, not electric - as in, it stems from a circulating magnetic field, not a (static?) electric field. And this is exactly how an "electromagnetic field" can be seen as comprising electric and magnetic components which will have more "prominence" (seem to be doing more of the work) in different reference frames, due to relativity.
	- So, whether you use Maxwell's equations + Lorentz law (?), or Coulomb's law + special relativity, you uncover the same outcome - the same force experienced by P.
- **Normal ordering**
	- Creation operators on the left, annihilation operators on the right.
	- A standard for writing a series of excitations ? or sequence of interactions ? represented by a bunch of creation/annihilation operators multiplied (i.e., performed on, operated upon, one another ?).
	- Why? In addition to standardisation in how stuff in QFT written, it also serves to eliminate infinities which are inherent in the hamiltonian operator arrived at after canonical quantisation (due to integrating over the Dirac delta function ?)
- Copenhagen interpretation (orthodox)
	- If particle measured at C, where was it before?
	- if particle measured at C, it's because observation/measurement collapsed wavefunction
	- vs realist (if particle measured at C, it was at C before)
	- vs agnostic (can't know - metaphysical, pejoratively)


# Converge
My current best representation/integration of everything I've diverged on above (and in the log below).

**Abbreviations**
- ED = (classical) electromagnetism/electrodynamics
- QED = quantum electrodynamics
- QM = quantum mechanics
- SR = special relativity
- QFT = quantum field theory

**List of Statements**
Exposition of current understanding.

"study" = "area concerned with...", "discipline", "area", "field"
Basically, TM uses "X studies Y" to refer to what (Y) a certain "area" (X) pertains to, including its objects of interest, tools it employs to investigate and understand these objects, etc.

## History of Developments
1. The Lorentz covariance of Maxwell's equations motivated the development of SR.
	1. Maxwell's equations do not transform consistently (covariantly) ? under <!--c:dqsej-->Galilean transformations<!--/c:dqsej-->. Lorentz came up with the Lorentz transformations, under which Maxwell's equations *do* transform covariantly. This Lorentz covariance of Maxwell's equations implied either (1) the existence of some "ether" which is considered a sort of universal rest frame ==?== or (2) the universality of the speed of light; this sparked Einstein to entertain the possibility of (2), which led to the development of SR.

## General Statements
1. Lorentz **invariance** can be thought of as a subset or special case of Lorentz **covariance**.

# SoC


[[Tue 28-07-2026]]
I want to understand the relations between these: classical field theory, QFT, quantum mechanics, special relativity, QED, electromagnetism, electrodynamics, anything else relevant that links these.

Here is an exposition of my current understanding:
"Electromagnetism" refers to the general phenomena associated with electric and magnetic fields. "Electrodynamics" refers to a subset of these in which there is *movement* (hence "dynamics") and in this case, very roughly/imprecisely/naively, this specifically means moving charge, or moving magnet ? (magnetic dipole ?)
This is *classical* electrodynamics, which is itself a *classical* field theory, in contrast to a *quantum* field theory, which incorporates the probabilistic (or, indeterministic) nature of quantum mechanics, where classical field theory (CFT?) is deterministic and so is invalid when considering the indeterministic "class of phenomena" ? that occur at the quantum scale (Planck scale ? what is correct term for the scale at which classical should be modelled as quantum, and how does this relate to e.g. Compton and de Broglie wavelengths?)
So, a QFT unifies CFT, special relativity and QM. CFT, at least with electromagnetism, is naturally relativistic because it concerns light ? but other CFTs not necessarily ? So, QFT is needed because QM is *non-relativistic* and so any phenomena associated with relativity (e.g. mass-energy equivalence, space contraction, ? I need to clarify which phenomena actually make the transition from QM to QFT necessary / are relevant here) are not represented. And in the other direction, QFT is needed because EM is *deterministic* because it addresses non-quantum scales (macroscopic phenomena ?) and so any phenomena associated with "unpredictability of behaviour" at the quantum scale is not represented by EM alone.

Ultimately, I'm trying to understand where each area fits into the picture - so, what are the deficiencies of each, for which others must be incorporated to supplement? To understand the "ingredients" necessary for a comprehensive, accurate, holistic theory of electromagnetic phenomena, consistent at all scales (in all regimes) ? So, we need to account for (1) the indeterminism at the quantum scale (QM) and (2) the relativism at the speed of light (SR + EM), and these "characteristics" are able to coexist meaningfully & consistently in QFT (QFT is the "unifier").
I want to understand more about the general picture, as I've tried to represent above, but also more specific examples of actual phenomena that each theory alone would be unable to explain.
And then, I want to understand how all of this is represented mathematically, operationally - as in, how these different elements (e.g. indeterminism, relativism) are combined mathematically, and the role of literal *operators* and other objects of utility (e.g. Hermitian matrices). I want to map out which mathematical tools are used in which regime ? (representation, theory, such as classical EM, QM, QFT, SR) so I can see any overlap, and which are introduced *in order to* unify the necessary elements.
And on top of this, I want to understand where QED fits in it all. Because I've heard that QED is a theory of how matter couples with light (electrons and photons are the "key objects" that interact) but I don't know how this would map onto summarising QED as just e.g. the quantum representation/description of electromagnetic phenomena. Is that basically all QED is - a theory of EM that works at the quantum scale? Or are there additional insights/phenomena it accounts for that go beyond both EM and QM (hence the idea of coupling matter with light)? That is, is QED more than the sum of its (QM + EM + SR) parts? And why is it called "quantum electrodynamics" as opposed to "quantum electromagnetism", which I guess would be more general because does not imply the necessity of movement associated with "dynamics"?

As an aside, by what is generally considered Maxwell's 3rd equation (Faraday's law), a changing magnetic flux induces a circulating electric field (by which, I think means that the induced field encircles the object causing the changing magnetic flux, such as a magnet ?) and by the 4th equation (Ampere-Maxwell law), a moving charge induces a circulating magnetic field (by which, I think means that the induced magnetic field encircles the moving charge, or current?). What are the different, concrete ways this actually occurs? For example, a solenoid - is this an instance of the 4th law, because a current passes through a coil, which induces a magnetic field *inside* the coil (because in this case, the current is circulating around a conductor ? and so the magnetic field must pass through it, at right angles? or, the magnetic field encircles the circles that are the wire through which the current runs?) I would like to enumerate and explicitise all the ways that Maxwell's equations apply, various common situations/setups in terms of how the electric/magnetic fields look, "slot together", which induces which, etc.






[[Tue 21-07-2026]]
Primary objective rn: understanding the bridge between classical and quantum ED. ACC, start with some representation of the classical formulation, via the Maxwell action ? which is gleaned from a Lagrangian density ?
and then this is "quantised" - but what's that? It means to take the Schrodinger equation, a continuous sort of probability distribution (density) ? to a discrete form - but what is that form?

15:30
? The Klein-Gordan equation is derived from the relativistic dispersion relation ? by substituting the quantities (energy and momentum) with their operator equivalents. For energy, this involves time derivative, and for momentum, the space derivative (Laplacian ?). Recall that the energy-momentum 4-vector has the components 1 = time, 2-3 = space.

But in order to get the KG equation, you need to square the ==dispersion== relation because otherwise, the time and space derivatives don't match (how? what?) - basically, the equation that just equates energy to the square root of (momentum^2 + mass^2), after substituting in the operators, doesn't work. Why? Idk yet. But when you *square* the relation, it works. But then, a problem arises: when you take the root to get the energy, obvs, a positive *and* negative component - but the idea of a negative energy is ==nonsensical==. So, the interpretation given by Feynman and ==?== is to view particles with a negative energy state as antiparticles, moving backwards in time. So, absorption of a negative-energy particle = emission of a positive-energy antiparticle ?

>nonsensical?

No, I don't think it's necessarily the fact that energy is negative, but that since energy is involved inthe time component of the probability current, it implies negative probability, and *that's* the nonsensical thing ? 

![[Pasted image 20260721155707.png|395]]

[[Mon 20-07-2026]]
"Electromagnetism" is an umbrella term for the phenomena associated with electric and magnetic waves, which could be thought of as 2 sides of the same coin - one cannot exist without the other.

Maxwell's equations relate electric and magnetic fields, describe their relationship, how they interact. Part of this relationship is the fact that a moving electric field induces a magnetic field, and a moving magnetic field induces an electric field. There's something to do with the induced fields being "circulating", which I think means literally circles around the "source" of the inducing field. Is it even accurate to say "moving electric field" in place of the probably more commonly used phraseology of "moving charge"? I would think so, because doesn't a charge create (instate? come along with?) an electric field, and so a moving charge is effectively just a moving electric field?

But actually, the fact that e.g. moving E-field induces moving M-field can be derived using simply Coulomb's law (for stationary charge, electrostatics?) plus special relativity. If you imagine a wire with equal number of positive and negative charges, moving in opposite directions (same velocity), by Maxwell's equations (classical EM), there will be a circulating magnetic field around this wire (because the fact there are charges moving represents a current?), and so a charge outside the wire moving at some velocity u (same or different to the charges inside) would experience a magnetic force (Lorentz force?) - or more precisely, a force from this apparent magnetic field. But if we take the perspective of the moving outsider charge (let's call P), and Lorentz transform to its reference frame, then the positive and negative charges inside the wire will have different velocities relative to this outside charge. So, from P's perspective, the wire is in fact charged (whereas from the original "laboratory" frame, the wire is neutral), and so P would, from its perspective, experience an electric force (Coulomb's law). But from the non-P perspective, this force is magnetic, not electric - as in, it stems from a circulating magnetic field, not a (static?) electric field. And this is exactly how an "electromagnetic field" can be seen as comprising electric and magnetic components which will have more "prominence" (seem to be doing more of the work) in different reference frames, due to relativity.

So, whether you use Maxwell's equations + Lorentz law (?), or Coulomb's law + special relativity, you uncover the same outcome - the same force experienced by P.

[[Fri 17-07-2026]]
Hermitian matrix is a matrix that is equal to its conjugate transpose. Hermitian matrices have certain properties that make them ideal for representing observables in physics - for example, position, momentum, kinetic energy, etc. An observable is just a physical quantity that can be measured at some point in time (in the lab, or in theory ? - in theory and/or practice?) One property is that they have real eigenvalues, and hence, these eigenvalues representing real quantities makes physical sense. Also, eigenvectors corresponding to distinct eigenvalues are orthogonal (can be normalised to make a set of orthonormal vectors?), so with Hermitian matrices, can form a basis that spans the Hilbert space.

Each eigenstate (eigenvector of the Hermitian operator) can be used to represent a state of the system. What is the system? The system can represent a singular particle.

So, you prepare a particle in a particular state, to have a particular wavefunction, which represents how that particle evolves over time. ?

You can solve the Schrodinger equation to find the wavefunction of a particle in one state (e.g. ground energy state), and then use the lowering/raising ladder operators to obtain all other states (all other rungs of the ladder of possible energy states).

[[Thu 16-07-2026]]
When does it make sense to say "where is the wave"?

If you continuously oscillate a string, the "wave" is constantly "changing position" so it doesn't make sense to ask where the wave is. Instead, it makes sense to talk of its *wavelength*. But if on the other hand, you send one pulse down the wave, it travels along as a (localised) hump in the string, so it makes sense to talk of the wave's position, instead of its wavelength (it is not periodic, so a wavelength doesn't make sense).

This relates to the uncertainty principle because if you e.g. prepare a particle state in which position is highly specified, this is like the case of the singular, non-periodic pulse, and so it doesn't make sense to speak of its wavelength (which encodes its velocity, and hence momentum?) so more specificity in position leads to more generality in momentum. On the other hand, if momentum is highly specified (in e.g. a sinusoidal wave, where velocity is constant ?) it makes little sense to speak of its position as it varies constantly through time, so we sacrifice arriving at a specific measurement for position.

**What are the fundamental objects defined in QM?**
Position and momentum, defined via the wave function?
The wavefunction represents the state of a particular particle, and how it evolves over time.

[[Mon 13-07-2026]]
In classical mechanics, particles have position q and momentum p. In quantum mechanics, we "promote" these quantities to become operators, $\hat{q}$ and $\hat{p}$ which act on wavefunctions. In the position representation, this is a wavefunction of position, and in the momentum representation, it is a wavefunction of momentum. We tend to go with the position representation so that $\psi = \psi(q)$.

Then, the operators are defined (dropping the hats) as:
- $q \psi = q \cdot \psi$
- $p \psi = -i \frac{d \psi}{dq}$

But in the momentum representation, the position operator becomes a differential operator (w.r.t. momentum, and with +i instead of -i).

From these definitions, the "canonical commutator" ? is $[q, p] = i$  because applying it to an arbitrary wavefunction that is well-behaved ? always yields $[q, p] \psi = i \psi$ so the $\psi$ can just be factored out.

Then, the vacuum $\ket{0}$ is defined by "insisting that it is annihilated" by all the annihilation operators $a_{\vec{p}}$ (there is one for each momentum state/value ?):
$$a \ket{0} = 0$$
for all p.

Then a **particle** is represented by acting a creation operator for a particular momentum (state?) $a^\dagger$ on the vacuum:
$$a^\dagger \ket{0} = \ket{\vec{p}}$$


**Eigenvalue equation**
$$H \vert{}\vec{p}\rangle = \omega_{\vec{p}} \vert{}\vec{p}\rangle$$
The $\ket{p}$ is an energy eigenstate of the system, which H acts upon to "extract its total energy", which is represented by the omega.

Where $\omega_{\vec{p}}^2 = \vec{p}^2 + m^2$ because we treat each particle as a simple harmonic oscillator ? 
But we can see the parallel with the relativistic dispersion relation $$E^2 = p^2 + m^2$$
which implies (or we can interpret) that $\ket{p}$ is a momentum eigenstate for a particle of mass m.




[[Fri 10-07-2026]]
?
Gauge invariance means that a system describes the same mathematical reality (represents the same mathematical structures) as another system, but eliminates redundancies (e.g. unnecessary objects) in its representation/description. Gauge invariance is used to package the E and B fields into the 4-vector A (potential) in a way that allows them to be transformed Lorentz covariantly. 
![[Pasted image 20260710080155.png]]
The choices of phi and A are not unique, so different values can correspond to the same E and B fields.


[[Wed 08-07-2026]]
A function: input number, output number.
A functional: input function, output number. 

I worked on some examples of functional derivatives:
![[Pasted image 20260708100923.png]]
from QFT for gifted amateurs.

The four-derivative $\partial_{\mu}$ is the relativistic generalisation of the gradient $\nabla$.

[[Tue 07-07-2026]]

The Levi-Civita symbol  $\varepsilon^{ijkl}$ is antisymmetric and is defined by its indices: even permutations (where an even number of swaps are made from 0123) = 1, odd permutations (where an odd number of swaps of digits 0123 are made) = -1, and 0 for all other terms.

Tensors
Rank = number of indices
"mixed" = some up, some down

The Lorentz group includes Lorentz transformations; quantities are **Lorentz covariant** if they transform appropriately under the elements of the Lorentz group.

The d'Alembertian operator is the 4-dimensional generalisation of the Laplacian. It is basically the Laplacian but with a 2nd order time derivative term:
![[Pasted image 20260707114456.png]]

Dynamics is how things very over time. So, in classical dynamics, we use Newton's equations; in electrodynamics (i.e. electromagnetism) we use Maxwell's equations; in quantum dynamics, we use Schrodinger's equation ?

**Probability vs probability amplitude**
Probability is a physical quantity extracted from probability amplitudes, which are calculated as an integral involving a wavefunction.

---
[[Mon 29-06-2026]]
I just did a problem sheet from this video on Lagrangians and Hamiltonians https://youtu.be/0DHNGtsmmH8?si=icGjz04BPs33en2L. Spent ~2 hours on it. This is the day I developed an initial understanding of what Lagrangian/Hamiltonian even is.