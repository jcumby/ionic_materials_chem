class: title, no-number
time: 0
# Lecture 3 - Ionic Conductivity

.footer[- [Return to course contents](overview.html#overview)
]

---

class: roomy
# Lecture summary
$\require{mediawiki-texvc}$

- Recap of defect types
- Ionic conductivity
- Conduction mechanisms
- Ionic migration paths
- Energetics of conduction

---

# Defect recap

![:vote](https://app.wooclap.com/SUJNYY/questionnaires/677e6679ab729ecc44fc41e2)

---

# Defect recap results

![:results](./quiz_results/current/defect_recap.png)

---

class: compact

**NaCl Schottky**
- Intrinsic defect (composition doesn't change) so formula mass change is 0
- Vacancies essentially create a hole in the structure, so density decreases

**AgCl Frenkel**
- Intrinsic defect
- Vacancies and interstitials created at the same rate, so density doesn't change significantly

**TiO2 substitution with Zr**
- Zr is heavier than Ti (91.224 vs 47.867) so formula mass will increase
- Zr<sup>4+</sup> is slightly larger than Ti<sup>4+</sup> so we might expect volume to increase slightly, but overall the density will increase
	- NOTE: I *wrongly* said Zr<sup>4+</sup> was smaller than Ti<sup>4+</sup> in the lecture - sorry!

**Shear phase in WO<sub>3</sub>**
- $\ce{WO\_{3} -> WO\_{3-x}}$, so the formula mass will decrease
- Shear phase formation is a substantial rearrangement which is driven by reducing the overall volume. The result is that decrease in volume far outweighs the decrease in formula mass, so density will increase.

---
class: compact



** Replacing O by F in CeO<sub>2</sub>**
- $\ce{CeO\_2 -> CeO\_{2-x}F\_{x}}$
- F is slightly heavier than O (18.998 vs 15.999) so formula mass will increase slightly
- Charge balance requires us to reduce some Ce<sup>4+</sup> to Ce<sup>3+</sup>. There are a few ways to imagine this with KV notation:
	1. Replacing $O^{2-}$ by $F^{1-}$ occurs directly during synthesis:
		- $\ce{O\_{O} + Ce\_{Ce} + H\_{2} + \frac{1}{2}F\_{2} -> F\_{O}^{\bullet} + Ce\_{Ce}^{'} + H2O}$
		- (H<sub>2</sub> and F<sub>2</sub> are used to balance the equation here, but a real experiment would use a different fluorinating reagent such as CeF<sub>3</sub>)
	2. As-synthesised CeO<sub>2</sub> is fluorinated by filling existing oxygen vacancies:
		- $\ce{V\_{O}^{\bullet\bullet} + Ce\_{Ce}^{'} + \frac{1}{2}F\_{2} -> F\_{O}^{\bullet} + Ce\_{Ce}^{x}}$
		- Note that the fluorite structure is often prone to anion vacancies due to the mismatch between ionic radii and the geometry (this is particularly prevalent when the cation can be reduced). We'll see why this again in lecture 6.
---

class: compact
# Conductivity

- Many ionic solids conduct electricity; due to *ionic* and/or *electronic* motion.
- Most ionic solids are electrically insulating/semiconducting (localised electrons)
--

- Ionic conductors are important!

.pull-center[

![Electric vehicle](./images/electric_vehicle.jpg# db maxh-4)| ![Gas sensor](./images/gas_sensor_H2.jpg# maxh-4 )
:---------:|:-----------:
Batteries ([Lecture 4](lecture4.html)) | Sensors 
![Li separation from seawater membrane](./images/separation_membrane.jpg# maxh-4 ) | ![Fuel cell stack](./images/bloom_energy_fuel_cell.jpg# maxh-4 )
Separation Membranes | Fuel Cells ([Lecture 6](lecture6.html))
]


---

class: roomy
# Origin of ionic conduction

- Ionic conductivity is dominated by **defects**
	- In an ideal crystal, ions can't easily move
	- vacancies and/or interstitials are the main charge carriers
--

- Conductivity, $\sigma = nq\mu$, where
	- $n$ is number of charge carriers
	- $q$ is charge
	- $\mu$ is the mobility of charge carriers
--

- In ionic solids, conductivity covers  $\ce{10^{-16}\ S\ m^{-1}\ \bond{-} 10^3\ S\ m^{-1}}$
	- most solids are limited to around $\ce{10^{-2}\ S\ m^{-1}}$
	- Liquid electrolytes typically $\ce{10^{-1}\bond{-} 10^3\ S\ m^{-1}}$

???

The Siemen $(S)$ is the unit of conductance and is the inverse of resistance, measured in Ohms $(\Omega)$.

---

class: roomy
# Measuring Conductivity

- For electronic conductors, this is simple:
	- Apply a voltage $(V)$ and measure the resulting current $(I)$
	- Resistance (in $\Omega$) is found through Ohm's law; $ V = IR $
	- Resistivity (in $\Omega\ cm$) of the material calculated from geometry
	
- Resistivity $\rho$ (in $\Omega\ cm$) = $\frac{1}{\text{Conductivity}\ \sigma\ \mathrm{(in\ S\ cm^{-1})}}$


.pull-center[
<video width="390" height="220" controls loop autoplay muted>
    <source src="./images/electron_conduction.mp4" type="video/mp4">
</video>
]


.footer[
- In reality, we normally use two wires for V and two for I
]

???

Resistance (in $\Omega$) depends on how much material there is; twice the length of material will give twice the resistance. Resistivity is a material property and therefore allows us to compare materials.

---

class: compact
# Measuring Ionic Conductivity

- Ions cannot flow round a circuit, so current drops with a constant applied voltage

.center[
<video width="390" height="220" controls autoplay muted>
    <source src="./images/ionic_conduction.mp4" type="video/mp4">
</video>
]

--


- Instead, we use an alternating voltage - this is called Impedance spectroscopy (see [lecture 5](./lecture5.html))


.center[
<video width="390" height="220" controls loop autoplay muted>
    <source src="./images/ionic_conduction_reverse.mp4" type="video/mp4">
</video>
]


???

For comparison, during cyclic voltammetry the voltage is continuously varied but over a much slower timescale than impedance spectroscopy.

At each measured point in a CV the current due to ionic motion is 0 A, but current still arises due to the chemistry occurring at the electrodes.


---

class: compact
# Ion migration mechanisms

Three 'main' mechanisms of ionic migration

## 1. Vacancy mechanism

Vacancies move throughout the lattice (atoms move into vacancy)

.center[
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

.center[
<video width="400" height="400" controls loop autoplay muted>
    <source src="./files/interstitial_migration.mp4" type="video/mp4">
</video>
]

---

# 3. Interstitialcy (knock-on) mechanism

Interstitial ions 'push' into a neighbouring site

.center[
<video width="400" height="400" controls loop autoplay muted>
    <source src="./files/interstitialcy_knock_on_migration.mp4" type="video/mp4">
</video>
]
---

# Vacancy, Interstitial or Interstitialcy?

![:vote](https://app.wooclap.com/SUJNYY/questionnaires/677e6e978c20adf28c85c796)

---

# Suggestions

![:results](./quiz_results/current/conductivity_distinction.png)

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

![Nasicon migration paths](./images/ionic_conduction_pathway_nasicon.gif# w-75pct absolute l-10pct)

.footer[
- [Y. Deng, *Chem. Mater.*, 2018, 2618.](https://doi.org/10.1021/acs.chemmater.7b05237)
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

- Defect mobility $(\mu)$ is a thermally-activated process:
$$ \mu = \mu_0 \exp \left( -\frac{\mathrm{E_a}}{\mathrm{RT}} \right) $$
- interstitial sites are higher energy than vacancies, so will be more mobile.

![Migration energy](./images/migration_energy.svg# w-50pct relative l-3-12th)

???

Here, $\mu_0$ is the mobility at 0 K, $E_a$ is the activation energy for migration, $R$ is the gas constant and $T$ is the temperature.

Inserting an atom into an interstitial site creates a high density region which is energetically unfavourable. Creating a vacancy is also unfavourable, but atoms can normally "relax" around the vacancy, reducing the enthalpic cost. This (usually) means creating an interstitial is more energetically costly than creating a vacancy. (Assuming the migration pathway goes through the same high energy state).

---

class: no-number
# Variation with temperature

As $\sigma = nq\mu$ and $\mu$ is thermally-activated,
$$ 
\begin{align}
\sigma &= nq\mu_0 \exp \left(-\mathrm{\frac{E_a}{RT}} \right) \\\\
       &= A \exp \left(-\mathrm{\frac{E_a}{RT}} \right) \\\\
\end{align}
$$

???

Here, $n$ is the number of charge carriers, and $q$ is the charge on the charge carrier. It is difficult to measure the carrier mobility $(\mu)$ directly, so these terms are combined into a single pre-exponential factor $A$.

--

![Nasicon conductivity vs temperature](./images/nasicon_arrhenius.jpg# w-third fr relative b-3)
Plotting $\ln \sigma$ *vs.* $\frac{1}{\mathrm{T}}$ should give a straight line
- more commonly we plot $\log_{10} \sigma$ *vs.* $\frac{1000}{\mathrm{T}}$ for high temperature measurements
- gradient is $\frac{-E_a}{R}$ (or $\frac{-E_a}{2303R}$ using base 10).

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

class: roomy
# Lecture recap

- Defects can give rise to ionic conduction
	- Occurs by three main mechanisms:
		- Vacancy hopping
		- Interstitial hopping
		- interstitialcy (knock-on) cooperation
- Ionic conductivity is thermally-activated
	- shows Arrhenius-like behaviour
- Different defects have different conduction energetics
	- Pathways can sometimes be determined experimentally



---

# Feedback

![:vote](https://app.wooclap.com/SUJNYY/questionnaires/677d2ca6deb91d7cf8d0326c)

.footer[- [Return to course contents](overview.html#overview)
]
