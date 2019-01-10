---

layout: post
title: 5) Torsinoal Load
date:  2019-01-11 23:30:00 +0900
categories:
- Engineering - Mechanics of Materials
feature_image: https://www.facebook.com/photo.php?fbid=1893189787425704&set=a.1893187554092594&type=3&theater
---

<center>1. Torsional Deformation of a Circular Shaft</center>

Consider a shaft $AB$ subjected at $A$ and $B$ to equal and opposite torques $\mathbf{T}$ and $\mathbf{T'}$.We pass a section perpendicular to the axis of the shaft through some arbitrary point $C$ [Fig. 5.1.].

![useful image](https://raw.githubusercontent.com/brandonkim12/brandonkim12.github.io/master/assets/mechanics_of_materials/fig_45.JPG)

<center>Fig. 5.1. Shaft subject to torques and a section plane at C</center>

The free-body diagram of portion $BC$ of the shaft must include the elementary shearing forces $d\mathbf{F}$, which are perpendicular to the radius of the shaft. These arise from the torque that portion $AC$ exerts on $BC$ as the shaft is twisted [Fig. 5.2.a]. The conditions of equilibrium for BC require that the system of these forces be equivalent to an internal torque T, as well as equal and opposite to $\mathbf{T'}$ [Fig. 5.2.b].

![useful image](https://raw.githubusercontent.com/brandonkim12/brandonkim12.github.io/master/assets/mechanics_of_materials/fig_46.JPG)

<center>Fig. 5.2. 
(a) Free body diagram of section BC with torque at C represented by the contributions of small elements of area carrying forces dF a radius r from the section center. 
(b) Free-body diagram of section BC having all the small area elements summed resulting in torque T.</center>



$$\int \rho dF = T \\ \int \rho(\frac{\rho}{c} \tau_{\text{max}} dA) = T \\ \underset{\text{polar moment of inertia}}{\frac{\tau_{\text{max}}}{c}\underline{\int \rho^2 dA}} = T$$

Since $ dF = \tau dA$, where $\tau$ is the shear stress on the element of area $dA$, we can write

$$\int \rho(\tau dA) = T \tag{5.1.}$$

At first, we have to study how the torsional deformation affects the form of shaft. 



$$\tau = G\gamma \\ \gamma = \frac{\rho}{c}\gamma_{\text{max}}$$



* References
  * R.C. Hibbeler, "Mechanics of materials",  Pearson, 10th ed., ch.5
  * Ferdinand P. Beer, Mechanics of Materials, 7th ed., ch.4

