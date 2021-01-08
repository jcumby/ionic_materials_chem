class: title, no-number

# Lecture 2 - defects

---

# Lecture summary
$\require{mediawiki-texvc}$

- Introduction to defects
- Types of defect
- Instrinsic and extrinsic defects
- Defect equations
- Ionic conductivity

---

class: compact, no-number

# Defects

**All** crystals contain defects of some sort, for example:
- Missing atoms (*vacancies*)
- Atoms in the 'wrong' place
	- *interstitials* (between lattice sites) or *substitutions* (different atom types)
- Extended defects of lines or planes of atoms (see lecture 5)

--

Defects are often the source of interesting properties

![corundum-based gems](./images/corundum_gems.jpg# w-7-12th db fl)

![Strength of iron-carbon alloy](./images/steel_strength.gif# w-4-12th db fr)

.footer[
- ~1% Substitution in $\ce{Al2O3}$
- Effect of interstitial carbon on iron properties
]

---

class: compact

# Defect amounts

The amount of defects is a fine balance of entropy and enthalpy
- Defects gain entropy but have a (often large) formation energy

![Defect formation energy](./images/defect_formation.png# w-6-12th l-2-12th relative)

Minimum in $\mathrm{\Delta G}$ depends on structure and bonding, but typically << 1%.


---


class: compact
# Types of defect

The three most common defect types in ionic solids are:


Vacancy | Interstitial | Substitution |
:-----|:----:|----:
![Vacancy defect](./images/mx_vacancy.png# w-90pct) | ![Interstitial defect](./images/mx_interstitial.png# w-90pct) | ![Substitutional defect](./images/mx_substitution.png# w-90pct)

--

Additionally, defects can be either 
- *intrinsic* (maintaining stoichiometry) or 
- *extrinsic* (non-stoichiometric)

---

class: no-number

# Intrinsic defects

Two of the most common stoichiometric defects are:

![Walter Schottky](./images/walter_schottky.jpg# w-10pct db fr relative t-50pct)
**Schottky**
- Charge-balanced combination of anion and cation vacancies

![Walter Schottky](./images/yakov_frenkel.jpg# w-10pct db fr)
**Frenkel**
- Ions displaced to interstitial sites



Defects observed depend on both structure type and atoms involved.

.footer[
- Top: [Walter Schottky (1886-1976)](https://physicstoday.scitation.org/doi/pdf/10.1063/1.3023533)
- Bottom: [Yakov Frenkel (1894-1952)](https://olemiss.edu/sciencenet/poronet/frenkel-bio.pdf)
]
---

# Schottky defects

- Typically occur when anions and cations have similar size (e.g. $\ce{NaCl}$ structure)
- Reduced density compared with the ideal material
- e.g. $\ce{NaCl}$ - equal numbers of $\ce{Na}$ and $\ce{Cl}$ vacancies

.pull-left[![NaCl Schottky Defect](./images/NaCl_schottky.png# w-70pct)]

.pull-right[
![:jmol 400, 300, 2, 2, 2, select (Na1)\<33\>; spacefill ionic; color atoms TRANSLUCENT 0.8 gray; spacefill 0.9; select (Cl1)\<15\>; color atoms TRANSLUCENT 0.8 lightgreen; spacefill 0.9](files/NaCl.cif)
]

???

Careful density measurements can be useful for determining Schottky defect concentrations around 1%, but difficult for smaller concentrations.

---

# Frenkel defects

- Smaller ion normally displaced
- Only one ion shows defect
- e.g. $\ce{AgCl}$ ($\ce{NaCl}$-type)
	- Smaller $\ce{Ag+}$ ion displaced to tetrahedral holes in CCP $\ce{Cl-}$ structure

.pull-left[![AgCl Frenkel Defect](./images/AgCl_frenkel.png# w-70pct)]

.pull-right[
![:jmol 400, 350, 1, 1, 1, unitcell OFF; select (Na1)\<13\>; spacefill ionic; color atoms TRANSLUCENT 0.8 gray](files/AgCl_interstitial.cif)
]


---

# Defect equations

Useful to write equation for defects, using **Kroger-Vink** notation:
- Normal chemical symbols used for atoms, and $\ce{V}$ for vacancies
--

- Subscripts denote lattice or interstitial ($\ce{i}$) sites
--

- Charges shown relative to the ideal host site:
	- $\ce{'}$ for $1-$, $\ce{''}$ for $2-$, etc.;
	- $\ce{\bullet}$ for $1+$, $\ce{\bullet\bullet}$ for $2+$, etc.;
	- $\mathrm{x}$ for no net charge (sometimes omitted)
--

- For example:
	- Na vacancy in NaCl: $\ce{V_{Na}{'}}$
	- Ag interstital in AgCl: $\ce{Ag_{i}^{\bullet}}$

---

# Defect equations (2)

Defect equations must balance for:
- mass (atoms)
- charge
- sites
	- positions created/destroyed must balance

---
	
# Examples
$\ce{AgCl}$ interstitial formation again:

$$ \ce{Ag\_{Ag} <=> Ag\_{i}^{\bullet} + V\_{Ag}{'} } $$

--

$\ce{NaCl}$ Schottky formation:

$$ \ce{Na\_{Na} + Cl\_{Cl} <=> V\_{Na}{'} + V\_{Cl}^{\bullet} + NaCl } $$

--

Easily extended to substitutions, e.g. substituting $\ce{Al^{3+}}$ with $\ce{Cr^{3+}}$ in $\ce{Al2O3}$ (ruby):

$$ \ce{ 2Al\_{Al} + Cr2O3 <=> 2 Cr\_{Al} + Al2O3 } $$



???

Another way to think about $\ce{NaCl}$ Schottky formation is displacing one $\ce{Na+}$ and one $\ce{Cl-}$ to a 'new' unit cell on the 
edge of the crystal.

Writing a iso-electronic subsitution with Kroger-Vink notation is somewhat unnecessary, but will hopefully serve as an introduction to substitution!

---

class: roomy

# Substitution

- Ions of similar size can often replace each other
--

- While an integer number are substituted across a crystal, the average can be non-stoichiometric
	- often represented by a variable such as $\ce{x}$:
	- i.e. Ruby is $\ce{Al\_{2-x}Cr\_{x}O3}\quad(0 \leq x \leq 2)$ 
--

- Substitution can dramatically affect properties:
	- e.g. $\ce{La\_{2-x}Sr_{x}CuO4}$:
		- semiconducting for $x = 0$
		- superconducting (below 40 K) for $x = 0.15$
	

---

# Extrinsic defects

Substitution can also drive formation of defects,
e.g. doping $\ce{NaCl}$ with $\ce{CaCl2}$:

Overall synthesis reaction:
$$ \ce{(1-2x)NaCl + xCaCl2 -> Na\_{1-2x}Ca\_{x}Cl} $$

Kroger-Vink notation:
$$ \ce{2 Na\_{Na} + CaCl2 <=> Ca\_{Na}^{\bullet} + V\_{Na}{'} + 2NaCl} $$

---
class: compact
# More complex example

Sometimes, substitution (or 'doping') can give rise to multiple potential defects.

For example, substitution of $\ce{La^{3+}}$ for $\ce{Sr^{2+}}$ in $\ce{LaCoO3}$ could occur:

- by creating oxygen vacancies;
$$ \ce{ 2La\_{La} + 2SrO + O\_{O} <=> 2Sr\_{La}{'} + V\_{O}^{\bullet\bullet} + La2O3 } $$
- or by oxidising $\ce{Co^{3+}}$ to $\ce{Co^{4+}}$
$$ \ce{ 2La\_{La} + 2SrO + \frac{1}{2} O2 + 2Co\_{Co} <=> 2Sr\_{La}{'} + 2Co\_{Co}^{\bullet} + La2O3 } $$

???

It is impossible to determine which defects form just from looking at the formula; it is necessary to measure them (e.g. determine the Co oxidation state); this is not always easy,
particularly for small numbers of defects!

---

class: compact

# Solid solutions

Frequently, substitutional defect concentrations can exceed 1%
- known as a 'solid solution'
- Very important for tuning properties *via* synthesis
- Often useful to think of the "average ion" properties at each site
	- e.g. ionic radius, resulting in *Vegard's Law*
		- Lattice parameter is weighted average of the end-members, e.g. $\ce{Al\_{2-x}Cr\_{x}O3}$:

.pull-left[	
![Vegard's Law in Al2-xCrxO3](./images/vegards_law_AlCr_2O3.jpg# w-80pct)
]
.pull-right[
![:jmol 400, 280, 1, 1, 1, polyhedra BONDS \(aluminium\); color polyhedra translucent gray;](files/Al2O3.cif)
]

???

The terms solid solution and doping are used interchangeably, but often depend on the specific research area.

Note in many areas (e.g. phosphor materials) small amounts of doping is denoted by a colon, e.g. $\ce{ScVO4:Bi}$ 
represents the same as $\ce{Sc\_{1-x}Bi\_{x}VO4}$.


---

# Non-stoichiometry

Some materials are naturally non-stoichiometric even without extrinsic defects

- Very common in transition metal compounds
	- multiple oxidation states available
- Example: $\ce{FeO}$ (wustite, $\ce{NaCl}$ structure) cannot actually form stoichiometrically at ambient pressure
	- Actually $\ce{Fe\_{1-x}O}$, with $0.05 \leq x \leq 0.15$
	
--

**N.B. From cation:anion ratio alone you cannot determine the defect types** <br>
e.g. Fe:O ratio of 0.9 could equally be $\ce{Fe\_{0.9}O}$ or $\ce{FeO\_{1.11}}$!

???

The exact composition formed is dependent on the exact synthesis conditions, in particular temperature (as higher temperature 
would cause the entropy term to dominate, assuming the product could be 'quenched' to room temperature).

---
class: roomy
# Conductivity

- Many ionic solids conduct electricity; due to *ionic* and/or *electronic* motion.
- Most ionic solids are electrically insulating/semiconducting (localised electrons)
--

- Ionic conductivity is dominated by *defects*
	- 'Ideal' lattice sites are fixed in place
- Conductivity, $\sigma = nq\mu$, where
	- $n$ is number of charge carriers
	- $q$ is charge
	- $\mu$ is the mobility of charge carriers
	
---

class: compact

# Ion migration mechanisms

Three 'main' mechanisms of ionic migration

## 1. Vacancy mechanism

Vacancies move throughout the lattice (atoms move into vacancy)

.pull-center[
<video width="350" height="350" controls loop autoplay muted>
    <source src="./files/vacancy_migration.mp4" type="video/mp4">
</video>
]

???

These are the most common suggested mechanisms, but others have been proposed in various materials (in particular cooperative 
mechanisms involving lattice vibrations [phonons] and multiple ion types).

---

# 2. Interstitial mechanism

Ions hop between interstitial sites

.pull-center[
<video width="400" height="400" controls loop autoplay muted>
    <source src="./files/interstitial_migration.mp4" type="video/mp4">
</video>
]

---

# 3. Interstitialcy (knock-on) mechanism

Interstitial ions 'push' into a neighbouring site

.pull-center[
<video width="400" height="400" controls loop autoplay muted>
    <source src="./files/interstitialcy_knock_on_migration.mp4" type="video/mp4">
</video>
]
---
name: migration_paths
# Migration paths


Ion paths are rarely .red[direct], but will take the .gold[lowest energy route].

.pull-left[
![:jmol 350, 350, 1, 1, 1, rotate x 100; 
rotate y 10; 
select (Na1)\<20\>; 
\(sodium\).radius=0.5; 
\(chlorine\).radius=1.0; 
color atoms TRANSLUCENT 0.8 gray; 
draw ID "observed" ARROW \(2.81 2.81 5.62\) \(4.2 4.2 4.2\) \(5.3 5.3 5.2\) WIDTH 0.3 COLOR orange; 
draw ID "direct" ARROW \(2.81 2.81 5.62\) \(5.2 5.2 5.62\) WIDTH 0.3 COLOR red](files/NaCl.cif)
]

.pull-right[
![Close-packed migration path](./images/migration_path_cp.svg# w-80pct)
]

---

class: compact

# Pathways can be complex

- Migration pathways can be calculated and/or experimentally determined

*e.g.* **NASICON** $\ce{Na+}$ conductor, $\ce{Na3Zr2(SiO4)2(PO4)}$:

![Nasicon migration paths](./images/ionic_conduction_pathway_nasicon.gif# w-100pct)

.footer[
- Y. Deng, *Chem. Mater.*, 2018, 2618.
]

???

Three approaches to determining diffusion are shown here:

**Molecular Dynamics (MD)**
- Computational model of ionic motion over a time period (using either electronic structure calculations or atomic potentials methods)
- Resulting trajectory is integrated to determine location of conducting ions

** Bond Valence Energy Landscape (BVEL) **
- Maps the bond valence sum (a measure of local electron density estimated from atomic positions) throughout the structure
- Surface is the region where the probe ion (e.g. Na<sup>+</sup>) would experience optimum coordination

** Maximum Entropy method (MEM) / Rietveld refinement**
- Fits a model to **experimental** data to determine ionic positions
- If Na<sup>+</sup> is diffusing throughout the measurement, the positional information is present within the
diffraction data. MEM is one method to fit this.

---

class:compact

# Migration energetics

- Defect mobility is a thermally-activated process:
$$ \mu = \mu_0 \exp \left( -\frac{\mathrm{E_a}}{\mathrm{RT}} \right) $$
- interstitial sites are higher energy than vacancies, so smaller energy barrier ($E_i < E_a$) - dominates

![Migration energy](./images/migration_energy.svg# w-60pct relative l-20pct)

---

class: compact, no-number

# Variation with temperature

As $\sigma = nq\mu$ and $\mu$ is thermally-activated,
$$ 
\begin{align}
\sigma &= nq\mu_0 \exp \left(-\mathrm{\frac{E_a}{RT}} \right) \\\\
       &= A \exp \left(-\mathrm{\frac{E_a}{RT}} \right) \\\\
\end{align}
$$

--

![Nasicon conductivity vs temperature](./images/nasicon_arrhenius.jpg# w-40pct fr relative b-1)
Plotting $\ln \sigma$ vs. $\frac{1}{\mathrm{T}}$ (or more commonly $\log_{10} \sigma$ vs $\frac{1000}{\mathrm{T}}$ for high temperature measurements) should give a straight line
- gradient = $\frac{-E_a}{R}$ (or $\frac{-E_a}{2303R}$).

.footer[
- 
- Nasicon conductivity
]


???

In reality, the number of defects increases with temperature, so both $\mu$ and $n$ have a T-dependence. 
Because defects have an associated formation energy $(\Delta \mathrm{H_{f}})$, it turns out that their formation is also thermally-activated
(it is possible to derive this from the defect formation equations, see e.g. West). In practice, it is common to plot $\log(\sigma T)$ vs $\frac{1000}{T}
to account for the T-dependence of A.

---

class: compact
# Lecture recap

- Crystals are never perfect!
	- defects favoured at higher temperature
- Three main types of defect:
	- vacancy (called Schottky if stoichiometry maintained)
	- interstitial (called Frenkel if stoichiometry maintained)
	- substitution
- Kroger-Vink notation is a way to write defect equations
- Some materials can form solid solutions and/or non-stoichiometric compositions
- Defects can give rise to ionic conduction
	- Occurs by three main mechanisms:
		- Vacancy hopping
		- Interstitial hopping
		- interstitialcy (knock-on) cooperation
- Ionic conductivity is thermally-activated
	- shows Arrhenius-like behaviour

