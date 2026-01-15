class: title, no-number

# Lecture 6 - Fuel cells

.footer[- [Return to course contents](overview.html#overview)
]

---

class: roomy
# Lecture Summary
$\require{mediawiki-texvc}$

- Fuel cell introduction
- Types of fuel cells
	- Polymer cells
	- Solid oxide fuel cells (SOFCs)
- Materials requirements for SOFCs
	- example materials
- Defect ordering

---

class: compact
# Fuel Cells

Fuel cells are similar to batteries; they have a cathode, electrolyte and anode.

![Fuel cell schematic](./images/fuel_cell_schematic.svg# w-50pct relative l-3-12th)

Electricity can be generated as long as fuel is supplied (they don't need to be recharged)

---

class: compact

![Fuel cell history](./images/fuel_cell_history.jpg# w-50pct absolute b-1 l-3-12th)

.footer[- [Handbook of Thermal Management Systems](https://doi.org/10.1016/B978-0-443-19017-9.00019-2), 2023
]


---

# Fuel cell fundamentals

$$
\ce{ {Fuel} + O2 -> H2O + nCO2}
$$

- Fuel cells grouped into *low-temperature* (LT, < 200 &deg;C) and *high-temperature* (HT, > 450 &deg;C). 

- H<sub>2</sub> is the preferred fuel 
	- Particularly for LT devices.
	- Doesn't produce CO<sub>2</sub>
--

- Other fuels (*e.g.* CH<sub>3</sub>OH, CH<sub>4</sub>, NH<sub>3</sub>) also possible
	- Steam reforming reaction converts fuels to $\ce{H2}$:
	$$\ce{CH4 + H2O ->[>700 ^{\circ}C] CO + 3H2}$$
		- can be achieved in-situ for HT cells, but must be separate for LT.
	
	
---

class: compact
# Fuel cell efficiency

Fuel cells are *very* efficient
- Convert fuel &rarr; electricity directly, rather than <br> 
fuel &rarr; heat &rarr; electricity (as in combustion)

$$
\text{Thermodynamic efficiency} = \frac{\Delta G}{\Delta H}
$$

*e.g.* for $ \ce{2H2 + O2 -> 2H2O} \ (\Delta H = -571.6\ \text{kJ mol}^{-1})$:

$$
\begin{align}
\text{Cathode:} & & \ce{4H+ + O2 + 4e- &-> 2H2O & & E} = +1.229 \mathrm{\ V} \\\\
\text{Anode:} & & \ce{4H+ + 4e- &<- 2H2} & & E = 0.00 \mathrm{\ V} \\\\
\end{align}
$$
--
$$
\begin{align}
\Delta G &= -nFE \\\\
         &= -4 \times F \times 1.229 \\\\
		 &= -474.3 \mathrm{\ kJ\ mol^{-1}} \qquad (\mathrm{per\ mole\ O_2})
\end{align}
$$
--
Efficiency = &eta; = -474.3 / 571.6 = **83%**

---

class: compact
# Thermodynamic Efficiency

$$
\Delta G = \Delta H - T\Delta S, \quad
\therefore \quad
\frac{\Delta G}{\Delta H} = \eta = 1 - \frac{T \Delta S}{\Delta H}
$$

--

For 'ideal' combustion engine (heat engine) the maximum efficiency is the Carnot limit:
- $ \eta = \frac{T\_{\mathrm{hot}} - T\_{\mathrm{cold}}}{T\_{\mathrm{hot}}} $

--

![Fuel cell and heat engine efficiency versus temperature](./images/fuel_cell_efficiency2.png# w-50pct relative l-20pct)

???

A heat engine is one that converts heat into work, for instance by repeatedly heating and cooling a substance while extracting (usually 
mechanical) motion. The term covers a huge range of technologies including combustion engines, thermal power stations and fridges (a heat pump, 
which is a heat engine operating in reverse).

A really nice example (in which the heating/cooling is done on a sealed chamber of air) is the Stirling engine:

<iframe width="560" height="315" src="https://www.youtube.com/embed/taDHMw38aE0" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

---

class: compact
# Types of fuel cell

Type | Mobile ion | Temperature (&deg;C) | Applications
-----|------------|--------------------------------|--------------
Alkaline | OH<sup>-</sup> | 50-100 | Stationary power, space missions
**Polymer**  | H<sup>+</sup> or OH<sup>-</sup> | 50-100 | Portable devices, transport
Phosphoric acid (PAFC) | H<sup>+</sup> | 220 | Medium to large scale combined heat and power (CHP) systems
Molten Carbonate (MCFC) | CO<sub>3</sub><sup>2-</sup> | 650 | &vellip;
**Solid Oxide (SOFC)** | O<sup>2-</sup> | 500 - 1000 | &vellip;

.footer[ - [L. Carrette, *Fuel Cells*, 2001, 5.](https://doi.org/10.1002/1615-6854(200105%291:1%3C5::AID-FUCE5%3E3.0.CO;2-G)
]

---

class: no-number
# Low temperature:<br> Proton exchange membrane fuel cell (PEMFC)

- Carbon electrodes with precious metal catalysts (Pt, Pd, Ru)
- Requires acidic proton-conducting polymer
	- *e.g.* Nafion
- Use H<sub>2</sub> as fuel, but can work with MeOH (less efficiently)

![Nafion structure](./images/nafion.png# w-40pct fl db)
![Gemini space craft](./images/gemini_spacecraft.jpg# w-50pct db fr)

.footer[
- Nafion
- Gemini spacecraft
]

???

Sometimes also known as polymer electrolyte membrane fuel cell

---

class: compact
# PEMFC + H<sub>2</sub>

$$
\begin{align}
\text{Anode:} & & \ce{2H+ + 2e- &<- H2} & & E = 0\ \mathrm{V}\\\\
\text{Cathode:} & & \ce{O2 + 2H+ + 2e- &-> H2O2} & & E = 0.695\ \mathrm{V} \\\\
& & \ce{H2O2 + 2H+ + 2e- &-> 2H2O} & & E = 1.776\ \mathrm{V}\\\\
\text{Cathode (Overall):} & & \ce{O2 + 4H+ + 4e- &-> 2H2O} & & E = 1.229\ \mathrm{V} \\\\
\end{align}
$$
--

- Good Low-temperature (< 100 &deg;C) operation .green[&#10004;]
	- Quick to start/stop
	- Suitable for portable applications
- H<sub>2</sub>O<sub>2</sub> forms when acidic .red[&#10008;]
	- Corrodes carbon-containing electrodes 
	- Lowers cell voltage
	- Requires expensive Pt or Pd catalysts to decompose H<sub>2</sub>O<sub>2</sub>
- Need careful hydration to ensure H<sup>+</sup> conduction  .red[&#10008;]


---

exclude: true
class: compact
# PEMFC + Methanol

Methanol easier to store/transport than H<sub>2</sub>
- Readily oxidised, does not require C-C bond breaking

$$
\begin{align}
\text{An.:} & & \ce{CO2 + 6H+ + 6e- &<- CH3OH + H2O} & & E = 0.046 \mathrm{\ V} \\\\
\text{Cat.:} & & \ce{\frac{3}{2}O2 + 6H+ + 6e- &-> 3H2O} & & E = 1.229 \mathrm{\ V} \\\\
\text{Overall:} & & \ce{ CH3OH + \frac{3}{2}O2 &-> CO2 + 2H2O} & & E= 1.183\mathrm{\ V}
\end{align}
$$
![PEMFC fuel cell](./images/PEMFC.jpg# db fr w-3-12th)

### Problems
- MeOH crosses from anode to cathode  .red[&#10008;]
	- Reduces cell voltage to ~0.5 V
- CO formed in side-reaction, blocking reaction sites  .red[&#10008;]
	- requires more Pt catalyst!


---

exclude: true
# Alkaline polymers?

- OH<sup>-</sup> as mobile ion prevents H<sub>2</sub>O<sub>2</sub> formation .green[&#10004;]
- pH change alters redox energies, allowing Ni catalysts to replace Pt .green[&#10004;]
- Attaching counter-cation to the polymer reduces electrode poisoning .green[&#10004;]

![Guanidimiszole alkaline polymer](./images/guanidimidazole_alkaline_polymer.jpg# w-60pct relative l-20pct)

- Current OH<sup>-</sup> polymers have low ionic conductivity! .red[&#10008;]

.footer[- [Y-J. Wang et al., *Chem. Soc. Rev.* **2013**, 42, 5768-5787.](https://doi.org/10.1039/C3CS60053J)
]

---

class: compact
# High temperature:<br>Solid Oxide (SOFC)

- All-solid-state system (*i.e.* solid electrolyte)
- Most work at 800 - 1000 &deg;C

--
- Based around redox and conduction of O<sup>2-</sup>:

$$
\begin{align}
&\text{Anode:} & &\begin{cases}
\ce{2H2O + 4e- &<- 2H2 + 2O^{2-}} \\\\
\ce{2CO2 + 4e- &<- 2CO + 2O^{2-}} \\\\
\ce{H2O + \frac{1}{2}CO2 + 4e- &<- \frac{1}{2}CH4 + 2O^{2-}} \\\\
\end{cases}  \\\\
&\text{Cathode:} & &\quad\ce{O2 + 4e- -> 2O^{2-}} \\\\
\end{align}
$$


--
- High temperature allows internal steam reforming; many fuels
- No precious metal catalysts
- Excess heat can be used to increase efficiency (to ~90%)
	- drive an electricity turbine or combined heat and power (CHP)



---

class: compact
# SOFC Limitations

High temperatures:
- prevent rapid start/stop
- cause reactivity between electrolyte and electrodes
- make thermal expansion important

--

Delicate balance between:
- optimum temperature for redox and/or ionic conductivity
- thermal expansion, reactivity and device construction
- Intermediate-temperature (IT) SOFCs are the current optimum.

![Commercial SOFC](./images/bloom_energy_fuel_cell.jpg# w-third relative l-30pct)

---

# Ideal requirements for fuel cell materials

Property | Anode              |       Electrolyte         |   Cathode
-------|-------------------|---------------------------|--------------
Electronic conductivity | High | Low | High
Ionic Conductivity | High | High | High
Chemical stability | reducing conditions | oxidising **and** reducing conditions | oxidising conditions
Catalytic activity | Fuel oxidation | (Fuel ox<sup>n</sup> and $\ce{O2}$ red<sup>n</sup>) | $\ce{O2}$ reduction

Also: chemical compatibility between materials, similar thermal expansion, low cost, ...

---

# Top Trumps - Fuel cell version


.pull-left.w30[
| $\ce{Bi\_{1.6}Gd\_{0.4}O3}$ ||
|-||
| ![:jmol 200,200,1,1,1, select NOT (oxygen); color atoms green; select (oxygen); color atoms translucent 0.5; select (all); color bonds white ](files/delta_Bi2O3.cif) |
| Electronic Conductivity | Low 
| Ionic Conductivity | High
| Oxidation Stability | Mid
| Reduction Stability | Low
]

.pull-left.w40.h-90p[
![:vote](https://app.wooclap.com/SUARKZ/questionnaires/6960f1c4328501edb3f27f55)
]

.pull-left.w30[
| MgO |
|-|
|  ![:jmol 200,200,1,1,1, select (all); color bonds white ](files/MgO.cif) |
| Electronic Conductivity | Low 
| Ionic Conductivity | Low
| Oxidation Stability | High
| Reduction Stability | High
]

---

exclude: False
# Top trumps #1 - answers

.pull-left[
Electrolytes should have high ionic conductivity, low electronic conductivity, and stability in both oxidising and reducing conditions.

Because MgO has low ionic conductivity it is not suitable as an electrolyte material, despite its good stability.
]

.pull-right[
![:results](./quiz_results/current/fuel_cell_TT1.png)
]



---
# Top trumps #2 


.pull-left.w30[
| $\ce{PrO_{1.833}}$ ||
|-||
| ![:jmol 200,200,1,1,1, select NOT (oxygen); color atoms green; select (oxygen); color atoms translucent 0.5; select (all); color bonds white ](files/Pr6O11.cif) |
| Electronic Conductivity | High
| Ionic Conductivity | Mid
| Oxidation Stability | ??
| Reduction Stability | ??
]

.pull-left.w40.h-90p[
![:vote](https://app.wooclap.com/SUARKZ/questionnaires/6964dc825eb1dfcad9388bf6)
]

.pull-left.w30[
| $\ce{Sr\_{0.89}Y\_{0.07}TiO\_{2.995}}$ |
|-|
|  ![:jmol 200,200,1,1,1, select (all); color bonds white; connect (strontium)(oxygen) DELETE; ](files/SrY_TiO3.cif) |
| Electronic Conductivity | High 
| Ionic Conductivity | Mid
| Oxidation Stability | Low
| Reduction Stability | High
]


---

exclude: False
# Top trumps #2 - answers


.pull-left[
Estimating stability to oxidation/reduction relies on considering the available oxidation states (particularly of the cations). 

$\ce{PrO\_{1.833}}$ has the formal oxidation state of Pr as +3.67 - you could equally write the formula as $\ce{Pr^{3+}Pr^{4+}\_2O\_{5.5}}$ (or $\ce{Pr^{3+}Pr^{4+}\_2O\_{6-x}}$ to imply it is fluorite-derived). 

This makes it clear that the material can be both oxidised (to $\ce{Pr^{4+}}$) and reduced (to $\ce{Pr^{3+}}$), giving it poor stability under both conditions.
]

.pull-right[
![:results](./quiz_results/current/fuel_cell_TT2.png)
]

---

# Top trumps #3


.pull-left.w30[
| $\ce{CsH(SO4)}$ ||
|-||
| ![:jmol 200,200,2,2,2, select (all); color bonds white;
moveto 0 \( -833 -381 -401 101.33\) 115.47 0.0 0.0; connect (caesium)(oxygen) DELETE; polyhedra BONDS \(sulfur\)](files/CsHSO4.cif) |
| Electronic Conductivity | Low
| Ionic Conductivity | ???
| Oxidation Stability | Mid
| Reduction Stability | Low
]

.pull-left.w40.h-90p[
![:vote](https://app.wooclap.com/SUARKZ/questionnaires/6964e3c25eb1dfcad93e4228)
]

.pull-left.w30[
| $\ce{(NH4)3H(SO4)2}$ |
|-|
|  ![:jmol 200,200,1,2,2, select (all); color bonds white; polyhedra BONDS \(sulfur\); moveto 0 \( -717 -489 -497 109.19 \) 132.25 0.0 0.0  ;](files/NH4_3_HSO4.cif) |
| Electronic Conductivity | Low
| Ionic Conductivity | ???
| Oxidation Stability | Mid
| Reduction Stability | Low
]

---

exclude: False
# Top trumps #3 - Answers

.pull-left[
$\ce{(NH4)3H(SO4)2}$ is a better ionic conductor than $\ce{CsH(SO4)}$, due to the structural arrangement of hydrogen bonds. In $\ce{CsH(SO4)}$ the conduction is within 2D planes separated by large Cs cations. In contrast, $\ce{(NH4)3H(SO4)2}$ has a 3D network of hydrogen bonds formed by the ammonium cations, allowing for more efficient proton hopping throughout the structure.

[This review](https://doi.org/10.1016/j.ijhydene.2011.09.152) gives more detail about proton-conducting solid acids.

]

.pull-right[
![:results](./quiz_results/current/fuel_cell_TT3.png)
]

---



class: compact
# 'Perfect' electrodes

Ideally, electrodes should be good electronic *and* ionic conductors!
- fuel/oxygen reactions would occur at the electrode surface

![Mixed conductor reaction sites](./images/triple_phase_boundary_mixedconductor.svg# w-third relative l-30pct) 

--

In reality, use a mixture of good ionic and electronic conductors.
- reactions occur at the **triple phase boundary**

![Electronically conducting electrode reaction sites](./images/triple_phase_boundary_electronic.svg# w-third relative l-30pct) 


---


# Typical anode materials

Usually a cermet (*i.e.* mixture) of Ni and electrolyte
- Ni &rarr; high e<sup>-</sup> conductivity and catalytic activity
	- but susceptible to poisoning by S (forming stable $\ce{NiS}$)
- High ionic conductivity from electrolyte

![cermet schematic](./images/cermet.jpg# w-third relative l-30pct)

---

class: compact
# Typical cathode materials

Composite of $\ce{La\_{1-x}Sr\_{x}MnO\_{3}}$ perovskite (LSMO) and electrolyte
- LSMO gives e<sup>-</sup> conduction and high catalytic activity
	- $\ce{Sr^{2+}}$ subtitution generates holes in valence band
- poor performance below 700 &deg;C .red[&#10008;]

--

.pull-right[
![:jmol 320, 320, 1,1,1, connect (lanthanum)(oxygen) DELETE;
connect (lanthanum)(lanthanum) DELETE;
connect (lanthanum)(nickel) DELETE;
polyhedra BONDS \(nickel\);
color polyhedra translucent green;
select \(Oi\);
color atoms TRANSLUCENT 0.8 red;
rotate x 90](files/La2NiO4_interstitial.cif)
]

Interest in mixed-conductors:
- $\ce{La\_{1-x}Sr\_{x}CoO\_{3-y}}$ <br> (perovskite with $\ce{V_{O}}$)
	- good ionic/electronic conduction
	- high thermal expansion
- $\ce{La2NiO\_{4+x}}$
	- 'layered' $\ce{O\_{i}}$ conductor
	- $\ce{2Ni\_{Ni} + \frac{1}{2}O2 <=> O\_{i}^{''} + 2Ni\_{Ni}^{\bullet}}$

---

class: compact
# Electrolyte materials

Most studied electrolyte is $\ce{Y\_{0.15}Zr\_{0.85}O\_{1.925} }$ (yttrium-stabilised zirconia, YSZ)
- defective fluorite structure
- $\ce{Y2O3 + 2Zr\_{Zr} + O\_{O} <=> 2 Y\_{Zr}^{'} + V\_{O}^{\bullet\bullet} }$
- Sc-doping also effective (but expensive)

.pull-right[
![:jmol 350,350,1,1,1, select \(fluorine\);
color atoms red;
select \(calcium\);
color atoms blue;
select (atomno=20);
color atoms green;
select (atomno=9);
color atoms TRANSLUCENT 0.8 red
](./files/CaF2.cif)
]

Another commercial material is $\mathrm{Gd\_{0.1}Ce\_{0.9}O\_{1.95}}$ (CGO)
- Better for lower temperature
	- e<sup>-</sup> conductor above 600 &deg;C
	
Many other materials, but issues with cost, stability, manufacturing...

---

class: compact, no-number
# Improving Ionic conduction

As $\sigma = nq\mu$, so  as [defects] &uarr;, $\sigma$ &uarr;

--

*However*, at high defect concentrations we can get **defect clusters**
- Local ordering of defects reduces mobility

--

*e.g.* in YSZ:
$(\ce{(1-x)ZrO2 + \frac{x}{2}Y2O3 -> Y\_{x}Zr\_{1-x}O\_{2-\frac{x}{2}} })$

.pull-left[![Conductivity vs defect concentration](./images/YSZ_conductivity_doping.png)]
.pull-right[ ![Defect ordering YSZ](./images/ysz_vacancy_ordering.gif) ]

.footer[
- Conductivity vs $x$ in YSZ
- Ideal arrangement for $x=0.5, \ce{Y2Zr2O7}$
] 


???

In YSZ, introducing two Yttrium atoms (x=2) results in the formation of one oxygen vacancy.
Locally, these are found to order; the optimum arrangement is for each OM<sub>4</sub> tetrahedron
to contain 2 Zr and 2 Y, with oxygen vacancies arranging in a 'grid-like'p pattern.

The figure (a) shows the the equilibrium arrangement for Y<sub>2</sub>Zr<sub>2</sub>O<sub>7</sub> (x = 0.5). 
Compare this with the ideal fluorite structure consisting of edge-sharing OM<sub>4</sub> tetrahedra, shown below:

![:width 30%](./images/fluorite.gif)

---

class: compact
# Long-range defect ordering

As discussed in Lecture 2, defects can undergo long-range order
- Temperature can induce order-disorder phase transition

### Example: Ba<sub>2</sub>In<sub>2</sub>O<sub>5</sub>
- Brownmillerite structure ($\ce{ABO\_{2.5}}$ perovskite with ordered $\ce{V\_{O}^{\bullet\bullet}}$)
- Large increase in $\sigma$ at phase transition

.pull-left[ ![:jmol 450,350,2,1,2, rotate y -45; set autobond off; connect (all) (all) DELETE; connect 0.5 2.7 (In) (O) CREATE; polyhedra RADIUS 2.7 \(indium\); color polyhedra translucent orange](files/Ba2In2O5_ICSD73937.cif)
]

![Brownmillerite conductivity](./images/brownmillerite_conductivity.jpg# w-20pct relative)


---


class: compact
# Lecture recap

- fuel cells operate like a battery with continous 'charge' supply
	- Many similar materials properties required
- different technologies work at different temperatures
	- advantages and disadvantages for both
- properties of electrolyte, cathode and anode must be optimised
- ideal electrodes would be ionically *and* electronically conducting
	- more commonly a mixture of materials is used
- Ionic conduction reaches a maximum with defect concentration
	- defect ordering occurs
- Defect ordering can give rise to new structure types

---

# Feedback

![:vote](https://app.wooclap.com/SUARKZ/questionnaires/677d2d23f7d5c8b84d16386d)
.footer[- [Return to course contents](overview.html#overview)
]


