class: title, no-number

# Ionic Materials

### Dr James Cumby
### james.cumby@ed.ac.uk

.footer[
- Room 269
- Try pressing 'h' for help!
]

---

# Course Overview
$\require{mediawiki-texvc}$

Lecture | Topic
--|-------------
1 | Introduction to ionic materials
2 | defects and ionic conduction
3 | Batteries
4 | Dielectric materials
5 | Fuel Cells 

## Recommended Reading

Basic Solid State Chemistry, A. R. West, *Wiley*, **1988** and references given during course.


---
# Lecture Summary

1. Introduction to ionic structures
	- recap crystal structures
	- Lattice energy and close packing
	- Ionic structure types

---
class: compact

# Introduction

'Ionic materials' consist of both cations and anions:

- Many inorganic solids
	- e.g. $\ce{Na+Cl-}$ and $\ce{Mg^2+SO_4^2-}$
--

- Organic salts
	- ammonium acetate $\ce{NH4+CH3COO-}$
	- [chlorphenirammonium maleate](https://www.nhs.uk/medicines/chlorphenamine-including-piriton/) (active part of Piriton&reg;)
	![Piriton API](./images/chlorphenirammonium_maleate_piriton_molecule.png# w-3-12th r-2 absolute t-20pct )
--
	
- (in)organic salts
	- Mono-/Di-/Tri-Sodium citrate $\ce{Na\_{x}C6H\_{8-x}O7}$ 
		- collectively used as E331 in food
		- $\ce{x}$ can be varied from 1&ndash;3
	![Trisodium citrate](./images/trisodium_citrate.png# w-20pct r-2 absolute t-60pct)
--
	
- Ionic liquids
	- Either organic or inorganic, these are liquid below 100 &deg;C

---
class: compact

# Why are they interesting?

- Large range of practical applications
	- important for energy storage, but lots of other applications!
	- ionic liquids are gaining attention for many applications
--

- High melting points due to Coloumbic energy (see [later](#ionic_bonding))
--

- Electrically insulating
	- Electronegativity differences promote localised electrons
	![Ceramic insulator](./images/ceramic_insulator.jpg# w-3-12th absolute t-50pct r-2)
--

- Usually hard, and often robust to harsh conditions
	- e.g. Synroc is used to encapsulate nuclear waste

![synroc](./images/synroc.jpg# w-33pct relative l-2-12th)



???

Ionic solids find applications in a huge number of places, including:
- Batteries
- Dielectrics / ferroics (e.g. piezoelectrics)
- Fuel cells
- Laser materials; $\ce{Cr-Al2O3}$
- Magnetic materials; $\ce{\gamma-Fe2O3}$ (for information storage), $\ce{YBa2Cu7O_{7-x}}$ (high-T superconductor)
- Catalysts; $\ce{Bi2MoO6}$
- Phosphors

Synroc is a mixture of titanium oxide minerals

---
class: compact

# We can divide solids into two categories:

.pull-left[
Molecular (e.g. paracetamol)
- Strong bonds within molecules
- Weaker intermolecular interactions
![:jmol 400, 300, 2, 1, 1](files/paracetamol.cif)

]

.pull-right[
Infinite (e.g. NaCl)
- Strong bonds between all atoms
- No discrete molecules
![:jmol 400, 300, 2, 2, 2](files/NaCl.cif)
]

We'll concentrate on **infinite materials**.

???
Infinite materials are probably the most widely studied in terms of a broad range of ionic properties,
but it is important to realise that there are a number of important appplications (and research into)
molecular ionic materials, including:

- polymeric ionic conductors (for fuel cells)
- Molecular salts for phamaceutical applications
	- Often better *in-vivo* properties than e.g. co-crystals
- Ionic liquids for e.g. nuclear waste processing


---

# Recap on crystal structure

Periodic solids can be described by a unit cell
![Unit cell](./images/unit_cell.png# db center)

- Defined by lengths ($a$, $b$, $c$) and angles ($\alpha$, $\beta$, $\gamma$)
	- 'Lattice parameters'
--

- Possesses 'space group' symmetry (an extension to point groups)
--

- Atom positions defined by fractional position along lattice directions




???

## Space group symmetry
Space group symmetry extends the idea of point groups to include translational symmetry (adding 'glide planes' and 'screw axes'
to the more familiar symmetry elements such as mirror planes and rotations). The combination of **all** possible symmetry combinations
generates a finite number (230) of space groups.

---
class: compact

# Example: Sodium chloride

.pull-center[
![:jmol 500, 300, 1, 1, 1](files/NaCl.cif)
]

 | |
----------------|---|--
Cubic structure | $a = b = c = 5.62\ \AA{}$, $\alpha = \beta = \gamma = 90^\circ$  |
Spacegroup      | $\mathrm{Fm\bar3 m}$ (#225, point group = $\mathrm{O_h}$) |
Na atoms at:    | (0 0 0)       &emsp; (&half; &half; 0) &emsp;  (&half; 0 &half;) &emsp;  (0 &half; &half;) | (all symmetry-related)
Cl atoms at:    | (&half; 0 0)  &emsp; (0 &half; 0)      &emsp;  (0 0 &half;)      &emsp;  (&half; &half; &half;) | (all symmetry-related)

Because of symmetry, we only need to define one Na and one Cl position.
---

name: ionic_bonding

# Ionic Bonding

- Ionic compounds stay together because of electrostatic interactions (strong)
--

- Total electrostatic energy is the (infinite) sum over *all* ion pairs,
$$ E\_{\mathrm{Madelung}} = \sum_{i \neq j} \frac{q_i q_j}{4\pi \epsilon_0 r} $$
	$q$ is the charge on ions $i$, $j$ and $r$ is the distance between them
--

- $\frac{1}{r}$ dependence makes long-range interactions important

.footer[
- see Chem 1-states of matter for a recap on ionic compounds]

	
???
- One assumption here is that the ions act as hard spheres with integral charges; less valid for highly polarisable ions
- $\epsilon_0$ is the permittivity of free space

	
---

class: compact

# Infinite summations

- For infinite solids, periodicity usually means the sum converges
	- As $r$ increases, the contribution becomes smaller.
--

- An infinite sum can therefore be replaced by the Madelung constant
	- depends on the structure type
--

- e.g. for $\ce{NaCl}$:
$$
\begin{align}
E\_{\mathrm{Madelung}} &= \sum_{i \neq j} \frac{q_i q_j}{4\pi \epsilon_0 r} \\\\
&= \frac{\mathrm{N_A} q_i q_j}{4\pi \epsilon_0 r} \left( 6 - \frac{12}{\sqrt{2}} + \frac{8}{\sqrt{3}} - \frac{6}{2} + \frac{24}{\sqrt{5}} - ... \right) \\\\
&\simeq \frac{\mathrm{N_A} q_i q_j}{4\pi \epsilon_0 r} \times 1.74756
\end{align}
$$

???
- Whilst the infinite sum converges for some structures, for others it actually diverges (as the number of neighbours at distance $r \propto 4 \pi r^2$).
- Note that for $\ce{NaCl}$ the series shown (based on expanding $r$ as a sphere) has actually been proved to diverge, but I include it as it is conceptually easier to understand!
The correct value is obtained by expanding the cubic unit cell as a cube (rather than a sphere); this series does converge, but is more complex!

In reality, a number of methods exist to perform the summation, in particular the [Ewald Method](https://en.wikipedia.org/wiki/Ewald_summation) (commonly used in atomistic simulations) 

---
class: compact

# Ionic Structures

Generally, structures **maximise cation-anion** interactions (-ve energy) while **minimising like-charge** interactions (+ve energy)
- Maximise cation-anion coordination number
	- Ideally, ions should be densely packed
	
![Radius Ratio](./images/radius_ratio_cation_anion.png# w-4-12th relative l-4-12th)

In many materials, the optimum is found when the largest ion (often oxide) is **close-packed**

???
Although short-range electrostatics are important, the importance of long-range electrostatic interactions cannot
be ignored. Often, it is not possible to predict which structure will occur based just on local coordination number arguments


---

# Close packing

![Close packing animation](./images/close_packed_layers.png)

---

# Close packing

.pull-left[
Face-centered cubic (FCC)<br>
... .blue[A].green[B].gold[C].blue[A].green[B].gold[C] ...
<video width="400" height="350" controls loop autoplay muted>
    <source src="./images/fcc_animated.mp4" type="video/mp4">
</video>
]

.pull-right[
Hexagonal close-packed (HCP)
... .blue[A].green[B].blue[A].green[B].blue[A].green[B] ...
<video width="400" height="350" controls loop autoplay muted>
    <source src="./images/hcp_animated.mp4" type="video/mp4">
</video>
]


---

# Holes

CP arrangements of large (an)ions [X] leave 'holes' within the structure, which can be occupied by smaller (cat)ions [M]

![Close packing holes](./images/close_packed_holes.jpg# w-7-12th)

---
# Octahedral holes

One .gold[hole] per .red[cp ion] - both are 6-coordinate

.pull-left[

![:jmol 400, 300, 1, 1, 1, connect 3.5 (O) (Hole); color BONDS aliceblue](files/FCC_oct_holes.cif)
Rock salt (NaCl) structure
]

.pull-right[
![:jmol 400, 300, 2, 2, 1, connect 4 (O) (Hole); color BONDS aliceblue](files/HCP_octahedral_holes.cif)
Nickel Arsenide structure (e.g. FeS)
![Hard boild egg](./images/iron_sulfide_egg.jpg# w-4-12th fr)
]


---

# Rutile

Although not strictly close-packed, rutile (.gold[Ti].red[O<sub>2</sub>]) is distorted HCP
with $\ce{Ti^{4+}}$ filling half the octahedral holes
CN = .gold[6] / .red[3]

.pull-center[
![:jmol 400,300, 2, 2, 2, connect 3.5 (Ti) (O); color BONDS aliceblue ](files/rutile.cif)
]

---
# Tetrahedral holes

Two .gold[holes] per .red[cp ion]

.pull-left[
![:jmol 400, 300, 1, 1, 1, connect 3.5 (O) (Hole); color BONDS aliceblue](files/FCC_tet_holes.cif)
]

.pull-right[
![:jmol 400, 300, 1, 1, 1, connect 3.5 (O) (Hole); color BONDS aliceblue](files/HCP_tetrahedral_holes.cif)
]

Holes filled | FCC Type | CN(.gold[A]/.red[X]) |  | HCP Type | CN(.gold[A]/.red[X])
-------------|------|-------------|------------|---|----
All | Fluorite (.red[Ca].gold[F<sub>2</sub>]) | .gold[4]/.red[8] |  | (not possible) | -
Half | Zinc-blende (.gold[Zn].red[S]) | .gold[4]/.red[4] | &emsp; | Wurtzite (.gold[Zn].red[S]) | .gold[4]/.red[4]


---
class: compact

# Which structure type?

Generally, the structure formed depends on the ratio of ionic radii
- Smaller cations will prefer lower coordination numbers
	
$\frac{r^{+}}{r^{-}}$  |  Cation C.N.  | MX Structure | MX<sub>2</sub> Structure 
-----------------------|---------------|--------------|---------------------------
0.7 - 1.0              | 8             | $\ce{CsCl}$         | $\ce{CaF2}$
0.4 - 0.7              | 6             | $\ce{NaCl}$         | $\ce{TiO2}$
0.2 - 0.4              | 4             | $\ce{ZnS}$ (Wurtzite/Zinc-blende) | Anti-fluorite (e.g. $\ce{Li2S}$)


These are only approximate 'rules', and other binary structures exist (e.g. $\ce{CdI2}$, $\ce{CdCl2}$, $\ce{PbO}$, etc...)
- Very difficult to predict!


---
class: compact

# Beyond binary compounds

With 3 or more elements, structures become much more complicated!

An important one is perovskite, $\ce{ABX3}$
- $r(\mathrm{A}) \simeq r(\mathrm{X})$, so can be considered as FCC $\ce{AX3}$ layer with $\ce{B}$ filling 25% of octahedral holes:

.pull-left[![perovskite layer](./images/perovskite_layer.png# w-7-12th)]

.pull-right[
![:jmol 400, 300, 1, 1, 1](files/cubic_perovskite.cif)
]














