class: title, no-number
time: 0
# Lecture 2 - defects

.footer[- [Return to course contents](overview.html#overview)
]

---

time: 12
# Lecture summary
$\require{mediawiki-texvc}$

- Introduction to defects
- Types of defect
- Instrinsic and extrinsic defects
- Defect equations

---

class: compact, no-number
time: 54
# Defects

**All** crystals contain defects of some sort, for example:
- Missing atoms (*vacancies*)
- Atoms in the 'wrong' place
	- *interstitials* (between lattice sites) or *substitutions* (different atom types)
- Extended defects of lines or planes of atoms

--

Defects are often the source of interesting properties

![corundum-based gems](./images/corundum_gems.jpg# w-7-12th db fl)

![Strength of iron-carbon alloy](./images/steel_strength.png# w-4-12th db fr)

.footer[
- ~1% Substitution in $\ce{Al2O3}$
- Effect of interstitial carbon on iron properties
]

---

class: compact
time: 5:12
# Defect amounts

The number of defects is a fine balance of entropy and enthalpy
- Defects gain entropy but have a (often large) formation energy

![Defect formation energy](./images/defect_formation.png# w-6-12th l-2-12th relative)

Minimum in $\mathrm{\Delta G}$ depends on structure and bonding, but typically << 1%.


---

time: 464
class: compact
# Types of defect

The three most common defect types in ionic solids are:


Vacancy | Interstitial | Substitution |
:-----|:----:|----:
![Vacancy defect](./images/MX_vacancy.png# w-90pct) | ![Interstitial defect](./images/mx_interstitial.png# w-90pct) | ![Substitutional defect](./images/mx_substitution.png# w-90pct)

--

Additionally, defects can be either 
- *intrinsic* (maintaining stoichiometry) or 
- *extrinsic* (non-stoichiometric)

---

class: no-number
time: 612
# Intrinsic defects

Two of the most common stoichiometric defects are:

![Walter Schottky](./images/walter_schottky.jpg# w-10pct db fr relative t-50pct)
**Schottky**
- Charge-balanced combination of anion and cation vacancies

![Yakov Frenkel](./images/Yakov_Frenkel.jpg# w-10pct db fr)
**Frenkel**
- Ions displaced to interstitial sites



Defects observed depend on both structure type and atoms involved.

.footer[
- Top: [Walter Schottky (1886-1976)](https://physicstoday.scitation.org/doi/pdf/10.1063/1.3023533)
- Bottom: [Yakov Frenkel (1894-1952)](https://olemiss.edu/sciencenet/poronet/frenkel-bio.pdf)
]
---

time: 685
# Schottky defects

- Typically occur when anions and cations have similar size (e.g. $\ce{NaCl}$ structure)
- Reduced density compared with the ideal material
- e.g. $\ce{NaCl}$ - equal numbers of $\ce{Na}$ and $\ce{Cl}$ vacancies

.pull-left[![NaCl Schottky Defect](./images/nacl_schottky.png# w-70pct)]

.pull-right[
![:jmol 400, 300, 2, 2, 2, select (Na1)\<33\>; spacefill ionic; color atoms TRANSLUCENT 0.8 gray; spacefill 0.9; select (Cl1)\<15\>; color atoms TRANSLUCENT 0.8 lightgreen; spacefill 0.9](files/NaCl.cif)
]

???

Careful density measurements can be useful for determining Schottky defect concentrations around 1%, but difficult for smaller concentrations.

---

time: 770
# Frenkel defects

- Smaller ion normally displaced
- Only one ion type shows defect
- e.g. $\ce{AgCl}$ ($\ce{NaCl}$-type)
	- Smaller $\ce{Ag+}$ ion displaced to tetrahedral holes in CCP $\ce{Cl-}$ structure

.pull-left[![AgCl Frenkel Defect](./images/agcl_frenkel.png# w-70pct)]

.pull-right[
![:jmol 400, 350, 1, 1, 1, unitcell OFF; select (Na1)\<13\>; spacefill ionic; color atoms TRANSLUCENT 0.8 gray](files/AgCl_interstitial.cif)
]


---

time: 856
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

time: 1077
# Defect equations (2)

Defect equations must balance for:
- mass (atoms)
- charge
- sites
	- positions created/destroyed must balance

---

time: 1126
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

class: compact
# Quick test - $\ce{BaTiO3}$ Schottky Formation

$$
\ce{Ba\_{Ba} + Ti\_{Ti} + 3O\_{O} <=> V\_{Ba}{''} + V\_{Ti}{''''} +\ ?? + BaTiO3}
$$


![:vote](https://www.menti.com/ybwgg3gso4)

---

$$
\ce{Ba\_{Ba} + Ti\_{Ti} + 3O\_{O} <=> V\_{Ba}{''} + V\_{Ti}{''''} +\ ?? + BaTiO3}
$$

![:results](https://www.mentimeter.com/s/5da2441c8b1554ad6a8903da2cf46e83/be09f0058c0a)

---

class: roomy
time: 22:07
# Ionic Substitution

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

time: 24:46
# Extrinsic defects

Substitution can also drive formation of defects,
e.g. doping $\ce{NaCl}$ with $\ce{CaCl2}$:

Overall synthesis reaction:
$$ (1-2x)\mathrm{NaCl} + x\mathrm{CaCl}\_2 \rightarrow \mathrm{Na}\_{1-2x}\mathrm{Ca}\_{x}\mathrm{Cl} $$

--

Kroger-Vink notation:
$$ \ce{2 Na\_{Na} + CaCl2 <=> Ca\_{Na}^{\bullet} + V\_{Na}{'} + 2NaCl} $$

---
class: compact
time: 26:33
# More complex example

Sometimes, substitution (or 'doping') can give rise to multiple potential defects.

For example, replacing $\ce{La^{3+}}$ by $\ce{Sr^{2+}}$ in $\ce{LaCoO3}$ could occur:

--

- by creating oxygen vacancies;
$$ \ce{ 2La\_{La} + 2SrO + O\_{O} <=> 2Sr\_{La}{'} + V\_{O}^{\bullet\bullet} + La2O3 } $$
- or by oxidising $\ce{Co^{3+}}$ to $\ce{Co^{4+}}$
$$ \ce{ 2La\_{La} + 2SrO + \frac{1}{2} O2 + 2Co\_{Co} <=> 2Sr\_{La}{'} + 2Co\_{Co}^{\bullet} + La2O3 } $$

???

It is impossible to determine which defects form just from looking at the formula; it is necessary to measure them (e.g. determine the Co oxidation state); this is not always easy,
particularly for small numbers of defects!

---

# Quiz 2 - Extrinsic defects

At high pressure, oxygen vacancies in $\ce{Mg2SiO4}$ can react with $\ce{H2O}$ to form new defects.

![:vote](https://www.menti.com/2mdz9f9mvh)

---

# Results - Extrinsic defects

![:results](https://www.mentimeter.com/s/4a2eb2674200a5468dec683c4e2742e1/947fb0d5e600)

---


class: compact
time: 29:37
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

time: 32:55
# Non-stoichiometry

Some materials are naturally non-stoichiometric even without extrinsic defects

- Very common in transition metal compounds
	- multiple oxidation states available
- Example: $\ce{FeO}$ (wustite, $\ce{NaCl}$ structure) cannot actually form stoichiometrically at ambient pressure
	- Actually $\ce{Fe\_{1-x}O}$, with $0.05 \leq x \leq 0.15$
	
--

**N.B. From cation:anion ratio alone you cannot determine the defect types** <br>
e.g. Fe:O ratio of 0.9 could equally be $\mathrm{Fe\_{0.9}O}$ or $\mathrm{FeO\_{1.11}}$!

???

The exact composition formed is dependent on the synthesis conditions, in particular temperature (as higher temperature 
would cause the entropy term to dominate, assuming the product could be 'quenched' to room temperature).

---

time: 46:09
class: compact
# Defect ordering

- At large defect concentrations, defects can interact
    - minimises enthalpy
- Can occur as
	- clusters ('0D')
	- lines ('1D')
	- planes ('2D')

Often seen in microscopy, e.g. $\ce{ZrNb\_{24}O\_{62}}$ shows 2D order in two directions:

![Microscopy of shear structure in ZrNb24O62](./images/ZrNb24O62_shear_structures.png# w-6-12th l-3-12th relative)


---

# Example - $\ce{WO3}$

Plane-like defects often described as shear phases

.pull-left[
$\ce{WO3}$
![:jmol 400, 270, 10, 10, 1.5, polyhedra BONDS \(tungsten\);
color polyhedra translucent gray;
unitcell off;
rotate z 20;
zoom 180;
select none;
select add (all)\<624\>;
select add (all)\<628\>;
select add (all)\<560\>;
select add (all)\<556\>;
select add (all)\<481\>;
select add (all)\<485\>;
select add (all)\<406\>;
select add (all)\<410\>;
select add (all)\<338\>;
select add (all)\<342\>;
select add (all)\<263\>;
select add (all)\<267\>;
select add (all)\<188\>;
select add (all)\<192\>;
color atoms white;
draw plane1 ((all)\<481\>) ((all)\<485\>) ((all)\<267\>)
draw off;
#select WITHIN(-3.5\~ plane\~ @\(plane((all)\<481\> (all)\<485\> (all)\<267\>)\));
select WITHIN(-3.5\~ plane\~ $plane1);
color polyhedra translucent orange;
select none;
draw plane2 ((all)\<474\>) ((all)\<478\>) ((all)\<260\>);
draw off;
#select WITHIN(-3.5\~ plane\~ @\(plane((all)\<474\> (all)\<478\> (all)\<260\>)\));
select WITHIN(-3.5\~ plane\~ $plane2);
color polyhedra translucent green;
](files/cubic_WO3.cif)
]




.pull-right[
$\ce{WO\_{2.90}\ or\ W\_{10}O\_{29}}$
![:jmol 400, 270, 3, 3, 1, polyhedra BONDS \(tungsten\);
color polyhedra translucent gray;
unitcell off;
rotate x 90;
zoom 150;
select none;
draw plane3 ((all)\<470\>) ((all)\<730\>) ((all)\<650\>);
draw off;
select WITHIN(-3.5\~ plane\~ $plane3);
color polyhedra translucent green;
draw plane4 ((all)\<430\>) ((all)\<350\>) ((all)\<170\>);
draw off;
select WITHIN(2.5\~ plane\~ $plane4);
color polyhedra translucent orange;
](files/beta_WO3.cif)
]

---

class: compact
time: 53:10
# Lecture recap

- Crystals are never perfect!
	- defects favoured at higher temperature
- Three main types of defect:
	- vacancy (called Schottky if stoichiometry maintained)
	- interstitial (called Frenkel if stoichiometry maintained)
	- substitution
- Kroger-Vink notation is a way to write defect equations
- Some materials can form solid solutions and/or non-stoichiometric compositions
- If defects order, this can lead to new stoichiometric structure types



---

# Feedback

![:vote](https://www.menti.com/dxaabe4acm)

.footer[- [Return to course contents](overview.html#overview)
]
