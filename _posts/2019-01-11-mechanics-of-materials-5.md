---

layout: post
title: 5) Torsinoal Load
date:  2019-01-11 23:30:00 +0900
categories:
- Engineering - Mechanics of Materials
feature_image: https://www.facebook.com/photo.php?fbid=1893189787425704&set=a.1893187554092594&type=3&theater
---

<center>1. Torsional Deformation of a Circular Shaft and Torsion Formula</center>

Consider a shaft $AB$ subjected at $A$ and $B$ to equal and opposite torques $\mathbf{T}$ and $\mathbf{T'}$.We pass a section perpendicular to the axis of the shaft through some arbitrary point $C$ [Fig. 5.1.].

![useful image](https://raw.githubusercontent.com/brandonkim12/brandonkim12.github.io/master/assets/mechanics_of_materials/fig_45.JPG)

<center>Fig. 5.1. Shaft subject to torques and a section plane at C</center>

The free-body diagram of portion $BC$ of the shaft must include the elementary shearing forces $d\mathbf{F}$, which are perpendicular to the radius of the shaft. These arise from the torque that portion $AC$ exerts on $BC$ as the shaft is twisted [Fig. 5.2.a]. The conditions of equilibrium for BC require that the system of these forces be equivalent to an internal torque T, as well as equal and opposite to $\mathbf{T'}$ [Fig. 5.2.b].

![useful image](https://raw.githubusercontent.com/brandonkim12/brandonkim12.github.io/master/assets/mechanics_of_materials/fig_46.JPG)

<center>Fig. 5.2. 
(a) Free body diagram of section BC with torque at C represented by the contributions of small elements of area carrying forces dF a radius r from the section center. 
(b) Free-body diagram of section BC having all the small area elements summed resulting in torque T.</center>



$$\int \rho dF = T$$

Since $ dF = \tau dA$, where $\tau$ is the shear stress on the element of area $dA$, we can write

$$\int \rho(\tau dA) = T \tag{5.1.}$$

At first, we have to study how the torsional deformation affects the form of shaft. 

![useful image](https://raw.githubusercontent.com/brandonkim12/brandonkim12.github.io/master/assets/mechanics_of_materials/fig_47.JPG)

<center>Fig. 5.3. Description of Torsional Deformation</center>

At [Fig. 5.3.], we find that when the torque is applied, the longitudinal grid lines originally marked on the shaft tend to distort into a helix, [Fig. 5.3.], that intersects the circles at equal angles. Also, <u>all the cross sections of the shaft will remain flat</u>—that is, they do not warp or bulge in or out—<u>and radial lines remain straight</u> and rotate during this deformation. **Provided the angle of twist is small, then the length of the shaft and its radius will remain practically unchanged.**

Think about the one-end-fixed case, which is stated in [Fig. 5.4.]

![useful image](https://raw.githubusercontent.com/brandonkim12/brandonkim12.github.io/master/assets/mechanics_of_materials/fig_48.JPG)

<center>Fig. 5.4. Description of Torsional Deformation</center>

If the shaft is fixed at one end and a torque is applied to its other end, **then the dark green shaded plane in [Fig. 5.4.a] will distort into a skewed form as shown.** Here a radial line located on the cross section at a distance $x$ from the fixed end of the shaft will rotate through an angle $\phi(x)$. This angle is called *the angle of twist.* It depends on the position $x$ and will vary along the shaft as shown.

In order to understand how this distortion strains the material, we will now isolate a small disk element located at x from the end of the shaft, [Fig. 5.4.b.]. Due to the deformation, the front and rear faces of the element will undergo rotation—the back face by $\phi(x)$, and the front face by $\phi(x) + d \phi$. As a result, the difference in these rotations, $$d\phi$$, causes the element to be subjected to a shear strain, $\gamma$ (see Fig. 5.5.).

$$\int \rho(\frac{\rho}{c} \tau_{\text{max}} dA) = T \\ \underset{\text{polar moment of inertia}}{\frac{\tau_{\text{max}}}{c}\underline{\int \rho^2 dA}} = T \\ \tau = G\gamma \\ \gamma = \frac{\rho}{c}\gamma_{\text{max}}$$



* References
  * R.C. Hibbeler, "Mechanics of materials",  Pearson, 10th ed., ch.5
  * Ferdinand P. Beer, Mechanics of Materials, 7th ed., ch.4

