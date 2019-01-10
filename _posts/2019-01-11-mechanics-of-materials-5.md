---

layout: post
title: 5) Torsinoal Load
date:  2019-01-11 23:30:00 +0900
categories:
- Engineering - Mechanics of Materials
feature_image: https://www.facebook.com/photo.php?fbid=1893189787425704&set=a.1893187554092594&type=3&theater
---

<center>1. Torsional Deformation of a Circular Shaft and Torsion Formula</center>

* Torsional Deformation

Consider a shaft $AB$ subjected at $A$ and $B$ to equal and opposite torques $\mathbf{T}$ and $\mathbf{T'}$.We pass a section perpendicular to the axis of the shaft through some arbitrary point $C$ [Fig. 5.1.].

![useful image](https://raw.githubusercontent.com/brandonkim12/brandonkim12.github.io/master/assets/mechanics_of_materials/fig_45.JPG)

<center>Fig. 5.1. Shaft subject to torques and a section plane at C</center>

The free-body diagram of portion $BC​$ of the shaft must include the elementary shearing forces $d\mathbf{F}​$, which are perpendicular to the radius of the shaft. These arise from the torque that portion $AC​$ exerts on $BC​$ as the shaft is twisted [Fig. 5.2.a]. The conditions of equilibrium for BC require that the system of these forces be equivalent to an internal torque T, as well as equal and opposite to $\mathbf{T'}​$ [Fig. 5.2.b].

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

* Torsion Formula

Think about the one-end-fixed case, which is stated in [Fig. 5.4.]

![useful image](https://raw.githubusercontent.com/brandonkim12/brandonkim12.github.io/master/assets/mechanics_of_materials/fig_48.JPG)

<center>Fig. 5.4. Description of Torsional Deformation</center>

If the shaft is fixed at one end and a torque is applied to its other end, **then the dark green shaded plane in [Fig. 5.4.a] will distort into a skewed form as shown.** Here a radial line located on the cross section at a distance $x$ from the fixed end of the shaft will rotate through an angle $\phi(x)$. This angle is called *the angle of twist.* It depends on the position $x$ and will vary along the shaft as shown.

In order to understand how this distortion strains the material, we will now isolate a small disk element located at $x​$ from the end of the shaft, [Fig. 5.4.b.]. Due to the deformation, the front and rear faces of the element will undergo rotation—the back face by $\phi(x)​$, and the front face by $\phi(x) + d \phi​$. **As a result, the difference in these rotations, $$d\phi​$$, causes the element to be subjected to a shear strain, $\gamma​$ (see Fig. 5.5.).**

![useful image](https://raw.githubusercontent.com/brandonkim12/brandonkim12.github.io/master/assets/mechanics_of_materials/fig_49.JPG)

<center>Fig. 5.5. The Description for The Relationship Between The Shear Strain and The Angle of Twist</center>

In [Fig. 5.4.], we get the equations that 

$$\rho d \phi=dx\gamma \rightarrow \gamma=\rho \frac{d \phi}{dx} \tag{5.2.}​$$

Since $dx$ and $$d\phi$$ are the same for all elements, then $d\phi/dx$ is constant over the cross section, and (5.1) states that the magnitude of the shear strain varies only with its radial distance r from the axis of the shaft. Since $d\phi/dx = \gamma/\rho = \gamma_{\text{max}}/c$, then

$$\gamma = \frac{\rho}{c}\gamma_{\text{max}} \tag{5.3.}​$$

Since $\tau = G\gamma​$, we get

$\tau=(\frac{\rho}{c})\tau_{\text{max}} \tag{5.4.}​$

Combining (5.3.) and (5.4.), we get

$$\int \rho(\frac{\rho}{c} \tau_{\text{max}} dA) = T \\ \underset{\text{polar moment of inertia}}{\frac{\tau_{\text{max}}}{c}\underline{\int \rho^2 dA}} = T \tag{5.5.}​$$

Replacing the $\int \rho^2 dA​$ with $J​$, we get

$$\tau_{\text{max}}=\frac{Tc}{J} \tag{5.6.}​$$

$$\text{where}\begin{cases}\tau_{\text{max}} =& \text{the maximum shear stress in the shaft,} \\ & \text{which occurs at its outer surface} \\ T = & \text{the resultant internal torque} \\  & \text{acting at the cross section.} \\  & \text{value is determined from} \\ & \text{the method of sections and} \\ & \text{the equation of moment equilibrium} \\ & \text{applied about the shaft’s} \\ & \text{longitudinal axis} \\ J = & \text{the polar moment of inertia} \\ & \text{of the cross-sectional area} \\ c = & \text{the outer radius of the shaft} \end{cases}​$$

and

$$\tau=\frac{T\rho}{J} \tag{5.7.}$$

![useful image](https://raw.githubusercontent.com/brandonkim12/brandonkim12.github.io/master/assets/mechanics_of_materials/fig_52.JPG)

<center>Fig. 5.6. Circular shaft with stress elements at different orientations.</center>

<center> 2. Shear Stress Distribution.  </center>

If an element of material on the cross section of the shaft or tube is isolated, then due to the complementary property of shear, equal shear stresses must also act on four of its adjacent faces, as shown in [Fig. 5.7.a.]. As a result, the internal torque T develops a linear distribution of shear stress along each radial line in the plane of the cross-sectional area, and also an associated shear-stress distribution is developed along an axial plane, [Fig. 5.7.b.]

![useful image](https://raw.githubusercontent.com/brandonkim12/brandonkim12.github.io/master/assets/mechanics_of_materials/fig_50.JPG)

<center>Fig. 5.7. Description of Stress Distribution </center>

It is interesting to note that **because of this axial distribution of shear stress, shafts made of wood tend to split along the axial plane when subjected to excessive torque**, Fig. 5–8. 

![useful image](https://raw.githubusercontent.com/brandonkim12/brandonkim12.github.io/master/assets/mechanics_of_materials/fig_51.JPG)

<center>Fig. 5.8. Surficial Failure of Wood - Maximum Shear</center>

This is because wood is an anisotropic material, whereby its shear resistance parallel to its grains or fibers, directed along the axis of the shaft, is much less than its resistance perpendicular to the fibers within the plane of the cross section.



* References
  * R.C. Hibbeler, "Mechanics of materials",  Pearson, 10th ed., ch.5
  * Ferdinand P. Beer, Mechanics of Materials, 7th ed., ch.4

