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
* Physical mechanism of conduction: most easily explained by considering a gas and
  using ideas (Familiar from thermodynamics background)
* In the presence of a temperature gradient, energy transfer by conduction must then occur in the direction of decreasing temperature.
* The net transfer of energy by random molecular motion as a diffusion of energy.
* Heat transfer processes can be quantified in terms of appropriate rate equations.

![useful image](https://raw.githubusercontent.com/brandonkim12/brandonkim12.github.io/master/assets/thermodynamics_and_heat_transfer/fig_3.JPG)

<center>Fig. 3. Association of conduction heat transfer with diffusion of energy (molecular)</center>

![useful image](https://raw.githubusercontent.com/brandonkim12/brandonkim12.github.io/master/assets/thermodynamics_and_heat_transfer/fig_4.JPG)

<center>Fig. 4. 1-dimensional heat transfer</center>

$q_x''\,=\,-k\frac{dT}{dx}\,\,-(1)$ where $q_x''$ is the heat transfer rate in the $x$-direction per unit area perpendicular to the direction of transfer.