
time: 0
class: title, no-number
# Lecture 4 - Batteries

.footer[- [Return to course contents](overview.html#overview)
]

---

time: 37
class: roomy
# Lecture summary
$\require{mediawiki-texvc}$

- Electrochemistry fundamentals
- Battery history and overview
- Battery definitions
- Improving capacity
- Essential materials properties
	- types of electrode behaviour
- Effect of charging rate on capacity
- Galvanostatic measurements



---

class:compact
time: 1:47
# Essential electrochemistry

## Quantities

Throughout this course, we will see a number of electronics/electrochemistry terms, summarised here:

Term | Symbol | Description | Units
:-----|:-|:-|:-
Potential (or voltage) | E or V | the 'push' moving the electrons | Volts (V)
Current | I | the rate at which electrons move | Amperes (A)
Charge | Q | amount of electrons | Coloumbs (C) or Amp-hours (Ah, 1 mAh = 3.6 C)
Resistance | R | effects reducing the current | Ohms ($\Omega$)
Capacitance | C | ability to store charge | Farads (F)
Power | P | how much current, and with what force | Watts (W)

---

class: compact
time: 3:48
## Important relationships

Ohm's law - current and potential are linked:
$$ V = IR $$ (Ohm's law)
A current flowing for a period of time gives an overall charge:
$$Q = It$$
Power is a combination of current and voltage:
$$ P = IV $$
Resistivity $(\rho)$ and conductivity $(\sigma)$ are inversely related. Note that resistance $(R)$ is related to resistivity $(\rho)$ by accounting for the geometry of the object.
$$\rho = \frac{1}{\sigma}$$

???

$Q = It$ helps to understand why charge can have units of (m)Ah (particularly common in the battery literature)

---

time: 6:44
# Why batteries?

- Portable electronics
- Electric vehicles
- Grid-storage (e.g. from renewables)
- ...

Future batteries require more charge stored in a smaller volume and/or mass.

This requires *new materials* from chemistry.

![Renewable energy lightbulb](./images/renewable_energy_bulb.jpg# w-50pct relative l-3-12th)

---

time: 10:13
class: compact
# (Brief) Battery History ![Baghdad battery](./images/baghdad-battery-cutaway.jpg# fr w-20pct relative r-1)


- ***ca.* 190 AD**: Baghdad (or Parthian) battery
	- Iron and copper electrodes, filled with vinegar
--

- **1800**: Volta created the voltaic pile ![Voltaic pile](./images/VoltaBattery.JPG# w-20pct fr)
	- Alternating Ag and Zn discs, NaCl electrolyte
	- Enabled *chemistry* e.g. $\ce{2H2O -> H2 + O2}$
--

- **1836**: Daniell cell: <br>
$\ce{Zn|Zn^{2+}, SO4^{2-} || SO4^{2-} | Cu^{2+} | Cu}$
	- First practical electricity source (used to power telegraphs)
	![Daniell cell](./images/Daniell_cell_combined.jpg# w-20pct fr)
- **1859** Lead-acid battery (first rechargeable)
--

- **1886** The first dry cell: $\ce{Zn | NH4Cl | MnO2 }$
	- $\ce{NH4Cl}$ immobilised with plaster of Paris $(\ce{CaSO4 . {$0.5$} H2O})$
- **1899** The first alkaline battery: $\ce{NiO(OH) | KOH | Cd}$
--

- **1991** Li-ion battery commercialised by Sony



???

Voltaic pile came about as a disagreement between Volta and Galvani; the latter
had discovered that frogs legs would move when forming a circuit from two different types of metal.
Galvani asserted this was 'animal electricity'


---

time: 15:07
class: no-number, compact
exclude: false
# Chemistry Nobel prize 2019

[Awarded for contributions to the development of the Li-ion battery](https://www.nobelprize.org/prizes/chemistry/2019/popular-information/)

![Nobel medal](./images/Nobel_Prize.png# db absolute w-10pct t-2 r-2)
![Nobel prize 2019](./images/nobel_prize_2019.jpg# w-100pct)

.footer[
- Akira Yoshino
- M. Stanley Whittingham
- John B. Goodenough
]

???

Check out John Goodenough's laugh (always makes me smile)!

<iframe width="300" height="250" src="https://www.youtube-nocookie.com/embed/CkIKRoTFogU" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

---

time: 15:57
class: compact
# Definitions

.pull-left[![Battery charging schematic](./images/battery_charging_schematic.png# w-60pct fl)]
.pull-right[![Battery discharge schematic](./images/battery_discharging_schematic.png# w-60pct fr)]


Naming of *anode* and *cathode* is often unclear. Here we define:
- Cathode is **positive** electrode under **discharge** (being reduced)
- Anode is **negative** electrode under **discharge** (oxidised)

---

time: 17:13
# Main approaches

.pull-left[
### Cationic battery
Charge carried across electrolyte by cations
- $\ce{Li+, Na+}$ ...
- $\ce{Mg^{2+}, Ca^{2+}}$, ...
- Even $\ce{Zn^{2+}, Al^{3+}}$
]
.pull-right[
### Anionic battery
Anion charge carrier in electrolyte
- $\ce{OH-}$ (NiCd or NiMH)
- $\ce{F^{-}, Cl^-}$
- $\ce{HSO4-}$ (in Pb-acid)
]
![Battery types](./images/battery_types.png# w-80pct relative l-10pct)

???

Anionic batteries were historically important (e.g. $\ce{OH-}$ and $\ce{HSO4-}$) but have dropped out of favour
due to the focus on Li-ion batteries. $\ce{Na+}$ and $\ce{Mg^{2+}}$ batteries are currently in development, but 
some researchers are investigating alternative anions (e.g. $\ce{F-}$) to overcome some of the limitations.

---

time: 18:27
class: compact
# What makes a 'good' battery?

Perhaps the most important parameter in batteries is the total *energy capacity*, $\mathrm{E_{bat}}$
- Combination of cell voltage (*V*) and amount of charge (*Q*) stored in the material:
.red[$$
\mathrm{E_{bat}} = QV
$$]
.grey[*Q* is expressed in units of Ah, so *E*<sub>bat</sub> is in Wh (Watt-hours)]
--

- *E*<sub>bat</sub> is dependent on the amount of battery material. More useful are:
	- Specific (gravimetric) energy (Wh g<sup>-1</sup>). <br>
	  .grey[ Q per unit mass (Ah g<sup>-1</sup>)]
	- (Volumetric) energy density (Wh L<sup>-1</sup>). <br>
	.grey[ Q per unit volume (Ah L<sup>-1</sup>)]
	
???

Energy capacity is often also known as 'nominal energy' or just 'energy'. It is simply the amount of useful energy stored in the battery.

The total energy capacity depends on the size of the cell; e.g. an AA battery has ~ 2000 mAh @ 1.5 V (= 3 Wh), while an AAA has ~1000 mAh @ 1.5 V (= 1.5 Wh).
If you connected a 6 W LED lightbulb (equivalent brightness to a 40 W filament bulb) to them, an AA battery would last for 30 minutes, while an AAA would 
last for 15 minutes!

Because capacity depends on the cell size (amount of electrode material) the volumetric/gravimetric measures are better for comparing materials. 

Note that 1 Wh = 3600 J!
---

time: 20:42
# Improving batteries

Ideally, we want to maximise *both* volumetric and gravimetric energy densities
	
![Energy density](./images/cell_energy_density_mod.svg# w-100pct)
	

.footer[
- &copy; Barrie Lawson]


---

time: 22:12
# Approches to increase $\mathrm{E_{bat}}$

## 1. Increase *operating voltage*, $V$

![Battery energy diagram](./images/energy_diagram_schematic.png# w-60pct relative l-20pct)

Need large (+ve or -ve) electrode potentials: <br>
large electronegativity differences (e.g. $\ce{Li+, F-}$)

---

time: 24:35
class: compact
## 2. Increase *charge stored*, $Q$

The charge stored in a material can be calculated using Faraday's Law:
$$
Q_{\mathrm{theoretical}} = \frac{nF}{3.6 M_w}\qquad(\text{in mAh g}^{-1})
$$

--

*e.g.* for the cathode $ \ce{LiCoO_2 -> Li^+ + e^- + CoO_2} $:
--

$$
n = 1,
F = 96485.3 \: \mathrm{As\:mol}^{-1}, M_w = 97.873\: \mathrm{g\: mol^{-1}} \\\\
\therefore Q = 274\: \mathrm{mAh\: g}^{-1}
$$

--
In reality, the charge stored is less than the theoretical maximum

- CoO<sub>2</sub> is unstable: $ \ce{2Co^{IV}O_2 -> Co^{III}_2O_3 + \frac{1}{2}O_2} $
	- We can only safely reach Li<sub>0.5</sub>CoO<sub>2</sub>, so the useful capacity is 137 mAh g<sup>-1</sup>

???
	
Effectively, this is charge stored (nF) per formula mass. The factor 3.6 converts F from A.s mol^{-1}) into A.h mol^{-1}

NOTE: the total charge stored in a full cell is limited by the electrode with the smallest capacity (although this can
be overcome by using more/less of each material).

Clarification: during discharge, the $\ce{Li}$ is **removed** from $\ce{LiCoO2}$ (in contrast to the voice-over).
	
---

# Which will give the highest energy capacity

Which of the following cathode combinations will give the highest E<sub>bat</sub>?

Reaction | Potential vs. Li/Li<sup>+</sup> (V)
-------|--------------
$\ce{LiCoPO4 -> Li^+ + CoPO4 + e^-}$ | 4.7
$\ce{LiF + Ag^0 -> AgF + Li^{+} + e^{-}}$ | 4.1
$\ce{LiTiS2 -> Li^+ + TiS2 + e^{-}}$ | 2.0

.footer[
- Calculate per mole of reactants as written
]

---

# Vote

![:vote](https://www.menti.com/ab77octuab)

---

# Results

![:results](https://www.mentimeter.com/s/eeb2f2c2292ed89f112e9d23e2ce666d/4c39a964ddd3)

---

time: 28:09
# Ideal materials properties

Anode/Cathode | Electrolyte
-|-
High capacity for charge-carrying ion |           High ionic conductivity
Large potential difference (cell voltage) |       Low electronic conductivity
Good ionic and electronic conductor (ideally) |   Stable in contact with electrodes

--

Electrode materials fall into two categories:
- Conversion
- Intercalation




???

While electrodes should ideally be electronic conductors (to allow electrons to reach the reaction sites) in 
practice poor electron conduction can be overcome by additives (such as carbon particles)

Note that the terms intercalation and conversion have been derived from Li-ion battery research, but the 
ideas transfer to other technologies.


---

time: 30:28
class: compact
# Conversion electrodes

Electrochemical reaction proceeds during charge/discharge. <br>
As a general equation, 
$$
\ce{A\_{$a$}B\_{$b$} + ($b\times c$)C^{n} + ($nbc - am$)e- <=> aA^{m} + $b$BC\_{$c$}}
$$
--

## Examples:
Chloride-ion battery cathodes:
$$\ce{BiCl3 + 3Li+ + 3e- <=> Bi^{0} + 3LiCl} $$
Lithium-sulfur cathode (here, $a = 0)$:
$$\ce{S + 2Li+ + 2e- <=> Li2S  }$$
Metal hydride anode (used in NiMH):
$$ \ce{ H2O + M^0 + e- <=> OH- + MH } $$


???
The metal hydride example can be understood as $\ce{A = OH}$ and $\ce{B = H}$



---

time: 34:36
# Conversion electrodes (2)

### Advantages
- Wide range of reactions possible
	- could avoid scarce/expensive elements by using e.g. Fe, Cu, O...
- Large theoretical capacities
	- More than one charge carrier per heavy metal (see $\ce{BiCl3}$ example)

--

### Disadvantages
- Often low conductivity (ionic and/or electronic)
- Substantial volume changes during cycling
- Side reactions/dissolution of intermediate species


.footer[
- [Wu & Yushin, Energy Environ. Sci., 2017, 435.](https://doi.org/10.1007/s10008-017-3580-9)
]

---

time: 38:28
class: compact
# Intercalation electrodes

No chemical 'reaction'; mobile species is 'inserted' into a material able to accommodate its charge/size.

### Example: $\ce{Li_{$x$}CoO2}$

.pull-left[
![:jmol 400, 400, 3, 3, 1, polyhedra BONDS \(cobalt\); 
rotate x 90; 
color polyhedra translucent 0.7 blue; 
color lithium orange
color cobalt blue](files/LiCoO2.cif)
]

.pull-right[
- Close-packed hcp .red[oxygen] array
- .blue[$\ce{Co}$] occupies alternate layers of octahedral holes
- .gold[$\ce{Li+}$] can insert between Co layers, reducing $\ce{Co^{IV} <=> Co^{III}}$
	- Layer spacing varies with $x$
	- High $\ce{Li+}$ conductivity due to 2D vacancy-hopping mechanism
]

---

time: 40:40
class: compact
# Intercalation cathode families

 | 2D conductor | 3D conductor | 1D conductor
:---|:---:|:---:|:---:
Type | $\ce{\alpha-NaFeO2}$ | spinel | olivine
Structure | ![:jmol 200, 200, 3, 3, 1, polyhedra BONDS \(cobalt\); rotate x 90; color polyhedra translucent 0.7 blue; color lithium orange; color cobalt blue](files/LiCoO2.cif) | ![:jmol 200, 200, 1, 1, 1, polyhedra BONDS \(lithium\); color polyhedra translucent 0.7 orange; color lithium orange](files/LiMn2O4.cif) | ![:jmol 200, 200, 1, 2, 3, polyhedra BONDS \(iron\); polyhedra BONDS \(phosphorus\); select iron; color polyhedra translucent 0.7 brown; select phosphorus; color polyhedra translucent 0.7 green; color lithium orange; color iron brown; color phosphorus green; hide \< {lithium}.bonds \>; rotate x 90](files/LiFePO4.cif)
Formula | $\ce{LiCoO2}$ | $\ce{LiMn2O4}$ | $\ce{LiFePO4}$
$Q_{\mathrm{theo.}}$ / mAh g<sup>-1</sup> | 274 | 148 | 170

&#11164;&#129180;&#129180;&#129180;&#129180;&#129180;&#129180;&#129180;&#129180;&#129180;&#129180;&#129180;&#129180;&#129180;&#129180;&#129180;&#129180;&#129180;&#129180;&#129180;&#11164;    Better Li conduction    &#11164;&#129180;&#129180;&#129180;&#129180;&#129180;&#129180;&#129180;&#129180;&#129180;&#129180;&#129180;&#129180;&#129180;&#129180;&#129180;&#129180;&#129180;&#129180;&#129180;&#11164; <br>
&#11166;&#129180;&#129180;&#129180;&#129180;&#129180;&#129180;&#129180;&#129180;&#129180;&#129180;&#129180;&#129180;&#129180;&#129180;&#129180;&#129180;&#129180;&#129180;&#129180;&#129180;&#129180;&#129180;&#129180;&#129180;&#129180;&#129180;&#129180;&#11166;    Safer    &#11166;&#129180;&#129180;&#129180;&#129180;&#129180;&#129180;&#129180;&#129180;&#129180;&#129180;&#129180;&#129180;&#129180;&#129180;&#129180;&#129180;&#129180;&#129180;&#129180;&#129180;&#129180;&#129180;&#129180;&#129180;&#129180;&#129180;&#129180;&#129180;&#11166; <br>
&#11164;&#129180;&#129180;&#129180;&#129180;&#129180;&#129180;&#129180;&#129180;&#129180;&#129180;&#129180;&#129180;&#129180;&#129180;&#129180;&#129180;&#129180;&#129180;&#129180;&#129180;&#129180;&#129180;&#11164;    (Higher cost)    &#11164;&#129180;&#129180;&#129180;&#129180;&#129180;&#129180;&#129180;&#129180;&#129180;&#129180;&#129180;&#129180;&#129180;&#129180;&#129180;&#129180;&#129180;&#129180;&#129180;&#129180;&#129180;&#129180;&#129180;&#129180;&#11164; <br>


---

time: 43:55
class: compact
exclude: true
# Charging rates

A high $\mathrm{E_{bat}}$ is good, but we want to (dis)charge batteries quickly!
- Tradeoff between *Power* ($P=IV$) and $\mathrm{E_{bat}} (=ItV)$
- Seen on a Ragone plot:

![Battery ragone plot](./images/ragone_plot.svg# w-50pct relative l-3-12th)

.footer[
- [B.D. McCloskey, J. Phys. Chem. Lett., **2015**, 6, 3592.](https://doi.org/10.1021/acs.jpclett.5b01813)]

$\mathrm{E_{bat}}$ depends on the (dis)charge rate, so to compare different materials we use the $C\mathrm{-rate} = \frac{I}{Q}$
- e.g. for a 1000 mAh battery: $1C$ would sustain 1 A for 1 hour, $2C$ gives 2A for 30 mins, $\frac{C}{6}$ gives 0.167 A for 6 hours, etc.



---

time: 49:56
# Electrochemical measurements

To avoid variations in rate, battery analysis uses *Galvanostatic* (constant current) electrochemistry
- measure the resulting potential.
- easier to separate chemistry effects from rate effects

![Galvanostat graph](./images/galvanostat_graph.jpg# w-60pct relative l-20pct )



---

time: 51:38
# Electrochemical measurements (2)

*e.g.* for a 2.2 Ah battery:

.pull-left[![galvanostat example](./images/22Ah_battery_galvanostat.svg)]

--

.pull-right[![Potential versus capacity](./images/E_vs_capacity.svg)]

.pull-left[<br> Capacity is often expressed in a number of formats]

???

$\mathrm{E_{bat}}$ depends on the (dis)charge rate, so to compare different materials we use the $C\mathrm{-rate} = \frac{I}{Q}$
- e.g. for a 1000 mAh battery: $1C$ would sustain 1 A for 1 hour, $2C$ gives 2A for 30 mins, $\frac{C}{6}$ gives 0.167 A for 6 hours, etc.


---

time: 55:35
# Material insights from galvanostats

Solid Solution | Two-phase region 
---------------|------------------
![Voltage-capacity curve for solid solution](./images/voltage_curves_solid_soln.png# w-100pct) | ![Voltage-capacity curve for two-phase mixture](./images/voltage_curves_2phase.png# w-100pct) 
Ions can be continously added/removed from the material without a structural transition | Two distinct compositions exist together, and the relative proportions change with $x$

???

To a first approximation, the voltage depends linearly on the curvature of free energy with x,
$$
V \propto -\frac{\partial G(x)}{\partial x}.
$$
In the case of phase mixtures, the free energy follows a linear combination of the two phase minima,
 so the potential is constant.

![](./images/voltage_curves_free_energy.jpg# w-100pct)

For more information, see http://cpb.iphy.ac.cn/article/2016/1806/cpb_25_1_018210.html#close

---

time: 57:41 
class: compact
# Lecture recap

- we define cathode and anode under discharge conditions!
- two main categories of battery (based on mobile ion):
	- cationic or anionic
- we want to maximise	
	- Charge stored $Q$ in materials, and
	- operating voltage $V$
- Two types of electrode operation:
	- Conversion
		- wide range of chemistry, but problems with volume change and side reactions
	- intercalation
		- limited number of suitable materials
- we can understand the mechanism using galvanostatic electrochemistry



---

# Feedback

![:vote](https://www.menti.com/gdwftssnux)
.footer[- [Return to course contents](overview.html#overview)
]