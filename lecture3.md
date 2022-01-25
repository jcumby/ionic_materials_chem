class: title, no-number
time: 0
# Lecture 3 - Ionic Conductivity

.footer[- [Return to course contents](overview.html#overview)
]

---

time: 12
# Lecture summary
$\require{mediawiki-texvc}$

- Recap of defect types
- Ionic conductivity
- Conduction mechanisms
- Ionic migration paths
- Energetics of conduction

---

# Defect recap

![:vote](https://www.menti.com/xu5g5ogo27)

---

# Defect recap results

![:results](https://www.mentimeter.com/s/b263ad5a60b54a924a4c8a7399ae89b4/3dc6c5216a2c)

---

class: compact
time: 36:06
# Conductivity

- Many ionic solids conduct electricity; due to *ionic* and/or *electronic* motion.
- Most ionic solids are electrically insulating/semiconducting (localised electrons)
--

- Ionic conductors are important!


![Electric vehicle](./images/electric_vehicle.jpg# w-6-12th)| ![Gas sensor](./images/gas_sensor_H2.jpg# w-5-12th )
:---------:|:-----------:
Batteries ([Lecture 4](lecture4.html)) | Sensors 
![Li separation from seawater membrane](./images/separation_membrane.jpg# w-5-12th ) | ![Fuel cell stack](./images/bloom_energy_fuel_cell.jpg# w-5-12th )
Separation Membranes | Fuel Cells ([Lecture 6](lecture6.html))



---

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

- In ionic solids, conductivity covers  $\ce{10^{-16}\bond{-} 10^3\ S\ m^{-1}}$
	- most solids are limited to around $\ce{10^{-2}\ S\ m^{-1}}$
	- Liquid electrolytes typically $\ce{10^{-1}\bond{-} 10^3\ S\ m^{-1}}$
---


# Measuring Conductivity

- For electronic conductors, this is simple:
	- Apply a voltage (V) and measure the resulting current (I)
	- Link by Ohm's law; $ V = IR $
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

---

class: compact
# Measuring Ionic Conductivity

- Current flow is eventually restricted

.center[
<video width="390" height="220" controls autoplay muted>
    <source src="./images/ionic_conduction.mp4" type="video/mp4">
</video>
]

--


- Instead, we use alternating current
	- Impedance spectroscopy (see [lecture 5](./lecture5.html))

.pull-center[
<video width="390" height="220" controls loop autoplay muted>
    <source src="./images/ionic_conduction_reverse.mp4" type="video/mp4">
</video>
]

---

class: compact
time: 38:58
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

time: 39:53
# 2. Interstitial mechanism

Ions hop between interstitial sites

.pull-center[
<video width="400" height="400" controls loop autoplay muted>
    <source src="./files/interstitial_migration.mp4" type="video/mp4">
</video>
]

---

time: 40:24
# 3. Interstitialcy (knock-on) mechanism

Interstitial ions 'push' into a neighbouring site

.pull-center[
<video width="400" height="400" controls loop autoplay muted>
    <source src="./files/interstitialcy_knock_on_migration.mp4" type="video/mp4">
</video>
]
---

# Vacancy, Interstitial or Interstitialcy?

![:vote](https://www.menti.com/2h16y82x7w)

---

# Suggestions

![:results](https://www.mentimeter.com/s/4bdd96932d73ef5e1d1cb1bda1ade9b0/4e2c89b7d69c)

---

name: migration_paths
time: 42:58
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
time: 44:19
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
time: 47:42
# Migration energetics

- Defect mobility is a thermally-activated process:
$$ \mu = \mu_0 \exp \left( -\frac{\mathrm{E_a}}{\mathrm{RT}} \right) $$
- interstitial sites are higher energy than vacancies, so smaller energy barrier ($E_i < E_a$) - dominates

![Migration energy](./images/migration_energy.svg# w-60pct relative l-20pct)

---

class: compact, no-number
time: 50:03
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

time: 53:10
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

.footer[- [Return to course contents](overview.html#overview)
]

---

# Feedback

![:vote](https://www.menti.com/v1z7bmhzwv)

