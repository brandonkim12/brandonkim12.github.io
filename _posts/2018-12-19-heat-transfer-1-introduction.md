---
layout: post
title: 1) Introductions for the heat and mass transfer
date:  2018-12-19 23:30:00 +0900
categories:
- Engineering - Heat and Mass Transfer
feature_image: https://www.facebook.com/photo.php?fbid=1893189787425704&set=a.1893187554092594&type=3&theater
---

Why the mechanical engineer should know how the heat and mass is transferred? for mechanical engineers, it is essential for them to analyze:

- how the reaction between the mechanical components
- how the individual component or subsystem endures long for the given conditions
- how much mechanical power transmission occurs by heat and mass transfer

However, we don't know exactly what concept we need to take the heat and mass transfer. So, let us talk together what preliminaries are in need.

More detailed concepts would be found in thermodynamics post, so we just remind the things briefly.

<center>1. Nomenclatures</center>

- System, surroundings and boundary:

  - System: The space of $n$-th dimension, which contains all things what we want to analyze.
  - Surroundings: Everything excluding the system, whose dimension is also $n$-th one.
  - Boundary: The $(n-1)$-th-dimensioned distinguisher between system and surroundings.
  - Mainly we're involved in $n\,=\,3$

  e.g.) Control volume $\rightarrow$ system
  Whole world excluding system $\rightarrow$ surroundings
  Control surface $\rightarrow$ boundary

- Closed and Isolated System

  - Closed system: the system which always contain the same matter - no heat and mass transfer across its boundary.
  - Isolated system: a special type of closed system that does not interact in any way with its surroundings

* Heat transfer (or Heat)
  * Thermal energy in transit due to a spatial temperature difference.
  * Surface transfer phenomena
    There are three types of heat transfer: conduction, convection and radiation

![useful image](https://raw.githubusercontent.com/brandonkim12/brandonkim12.github.io/master/assets/thermodynamics_and_heat_transfer/fig_1.JPG)

<center>Fig. 1. How the conduction, convection and radiation occurs - brief diagram</center>

* Transport Phenomena
  * There are several topics for the transport phenomena:
  * Three levels at which transport phenomena can be studied
    * Macroscopic level - the equations for the macroscopic balance(mass, momentum, energy, and angular momentum), no attempt for the detailed stuffs
    * Microscopic level - the equations of change of above macroscopic values in microscopic region.
    * Molecular level - we seek a fundamental understanding of the mechanisms of mass, momentum, energy and angular momentum transport in terms of molecular structure and intermolecular forces.

![useful image](https://raw.githubusercontent.com/brandonkim12/brandonkim12.github.io/master/assets/thermodynamics_and_heat_transfer/fig_2.JPG)

<center>Fig. 2. Topics of transport phenomena</center>

Brief concepts of each the conduction, convection and radiation are below:

<center>2. Conduction</center>

* Atomic and molecular activity: processes at these levels sustain this mode of heat transfer
* Caused by the direct contact between the objects containing heat energy
* Physical mechanism of conduction: most easily explained by considering a gas and using ideas (Familiar from thermodynamics background)
* In the presence of a temperature gradient, energy transfer by conduction must then occur in the direction of decreasing temperature.
* The net transfer of energy by random molecular motion as a diffusion of energy.
* Heat transfer processes can be quantified in terms of appropriate rate equations.

![useful image](https://raw.githubusercontent.com/brandonkim12/brandonkim12.github.io/master/assets/thermodynamics_and_heat_transfer/fig_3.JPG)

<center>Fig. 3. Association of conduction heat transfer with diffusion of energy (molecular)</center>

![useful image](https://raw.githubusercontent.com/brandonkim12/brandonkim12.github.io/master/assets/thermodynamics_and_heat_transfer/fig_4.JPG)

<center>Fig. 4. 1-dimensional heat transfer</center>

* The heat flux $q_x''\,=\,-k \frac{dT}{dx}$ [Unit: $\frac{W}{m^2}$] where $q_x''$ is the heat transfer rate in the $x$-direction per unit area  perpendicular to the direction of transfer.
* The heat rate $q_x\,=\,q_x''\,\cdot A$ [W]
* The steady-state conditions (where the temperature distribution is linear), the temperature gradient may be expressed as $\frac{dT}{dx}\,=\,\frac{T_2\,-\,T_1}{L}$. (note the [Fig. 4.1] the meaning of each symbol)
  so, heat flux is expressed like $q_x''\,=\,k\frac{T_1\,-\,T_2}{L}\,=\,k\frac{\Delta T}{L}$

<center>3. Convection</center>

Due to random molecular motion and (diffusion), energy is also transferred by the bulk, or macroscopic, motion of the fluid.

* Convection:  customarily used when referring to this cumulative transport
* Advection: transport due to bulk fluid motion.
* Hydrodynamic Boundary Layer: The development of a region in the fluid through which the velocity varies from zero at the surface to a finite value $u_{\infin}$ associated with the flow, (consequence of the fluid–surface interaction.)
* Thermal Boundary Layer: A region of the fluid through which the temperature varies from at to in the outer flow as the surface and flow temperatures differ. 
  * may be smaller, larger, or the same size as that through which the velocity varies.

![useful image](https://raw.githubusercontent.com/brandonkim12/brandonkim12.github.io/master/assets/thermodynamics_and_heat_transfer/fig_5.JPG)

<center>Fig. 5. Boundary layer development in
convection heat transfer.</center>

* Forced convection: The flow is caused by external means. e.g.) a fan, a pump, or atmospheric winds.
* Natural convection: For free (or natural) convection, the flow is induced by buoyancy forces, which are due to density differences caused by temperature variations in the fluid.

* <u>**The most frequent form of heat transfer.**</u>

* In addition to energy transfer due to random molecular motion (diffusion), energy is also transferred by the bulk, or macroscopic, motion of the fluid. 

* The appropriate rate equation: $q''\,=\,h\begin{vmatrix}T_s\,-\,T_{\infty}\end{vmatrix}$. where $q''$ is the convective heat [$W/m^2$], $T_s$: surface temperature, $T_{\infty}$: fluid temperature

<center>4. Radiation</center>

Energy emitted by matter that is at a nonzero temperature. Regardless of the form of matter, the emission may be attributed to changes in the electron configurations of the constituent atoms or molecules.

* $$q''_{rad}\,=\,\frac{q}{A}\,=\,\epsilon E_b(T_s)\,-\alpha G\,=\,\epsilon\,\sigma(T_s^4\,-\,T_{sur}^4)$$
* $G_{abs}\,=\alpha\,G$ where $\alpha\,=\,$absoptity, $0≤\alpha≤1$

![useful image](https://raw.githubusercontent.com/brandonkim12/brandonkim12.github.io/master/assets/thermodynamics_and_heat_transfer/fig_6.JPG)

<center>Fig. 6. Radiation Exchange </center>

This property provides a measure of how efficiently a surface emits energy relative to a blackbody.

<br></br>

- References
  - Frank P. Incropera, "Fundamentals of Heat and Mass Transfer", 7th ed.
  - R. Byron Bird, Warren E. Stewart, "Transport Phenomena", 2nd ed.
  - Yunus A. Cengel, "Thermodynamics - An Engineering Approach", 8th ed.