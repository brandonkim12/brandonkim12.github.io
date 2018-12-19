---
layout: post
title: 1) Stress and Strain - Stress
date:  2018-12-11 23:00:00 +0900
categories:
- Engineering - Mechanics of Materials
feature_image: https://www.facebook.com/photo.php?fbid=1893189787425704&set=a.1893187554092594&type=3&theater
---


<center>-1. Stress and Strain</center>

Stress means the force acting on the unit area, such as $\sigma\,=\,\frac{F}{A} [\frac{N}{m}]\,=\,[Pa]$ where $F\,:\,Force,\,A\,=\,Area$.  

Strain means the difference between the initial length and final length for compared to the initial length, such as $\epsilon\,=\,\frac{L_0\,-\,L_f}{L_0}$. where $L_0$ is initial length of a specimen of a certain material, and $L_f$ is final length of the specimen. 

The mechanics of materials are the set of study for the relations between them. 



<center>-2. Preliminaries - statics</center>

* Equations of Equilibrium

Firstly, mechanics of materials deal with the static state, so we have two main formulas such that

$$\begin{align}& \sum \mathbb{F}\,=\,0 \\ & \sum \mathbb{M}_O \,=\,0\end{align}$$

In the most simple coordinates, in other words, cartesian coordinates, generally we deal with the xyz, so the above formula are expressed 6 formulas like below:

$$\begin{align} & \sum F_x\,=\,0, \sum F_y\,=\,0, \sum F_z\,=\,0 \\ & \sum M_x\,=\,0, \sum M_y\,=\,0, \sum M_z\,=\,0\end{align}$$

If you're in the two-dimensional situation, above 6 formulas are to be reduced to 3 formulas such as:

$$\begin{align}&\sum F_x\,=\,0 \\& \sum F_y\,=\,0 \\& \sum M_O\,=\,0 \end{align}$$



* Support Reactions

In statics, support options help us to solve the problem properly, sometimes are critical to define whether the problem could be solved.

![useful image](https://raw.githubusercontent.com/brandonkim12/brandonkim12.github.io/master/assets/mechanics_of_materials/fig_1.JPG)



<center>Fig.1 - Support options</center>



<center>-3. Forces used to analyze the stress and strain</center>

* Normal force: Force acts perpendicular to the area. 
* Shear force: Force makes the body to slide over one another.
* Torsional moment (or torque): The moment makes the body twist according to the perpendicular axis to the surface area.
* Bending moment: The moment makes the body bended

Abstract descriptions are below:

![useful image](https://raw.githubusercontent.com/brandonkim12/brandonkim12.github.io/master/assets/mechanics_of_materials/fig_2.JPG)



<center>Fig.2 - Force and moments acting on the body</center>

In many cases, we're going to deal with this picture:

![useful image](https://raw.githubusercontent.com/brandonkim12/brandonkim12.github.io/master/assets/mechanics_of_materials/fig_3.JPG)



<center>Fig.3 - Coplanar force and moment</center>



<center>-4. Stresses - Normal and shear stress</center>

![useful image](https://raw.githubusercontent.com/brandonkim12/brandonkim12.github.io/master/assets/mechanics_of_materials/fig_4.JPG)



<center>Fig.4 - Z-direction stresses</center>



* Normal Stress: stress for the normal force to a surface. For [Fig.4], $\sigma_z\,=\displaystyle{\lim_{\Delta A \to 0}}\frac{\Delta F_z}{\Delta A}$

* Shear Stress: stress for the shear force to a surface. For [Fig. 4], $\tau_{zx}\,=\displaystyle{\lim_{\Delta A \to 0}}\frac{\Delta F_x}{\Delta A}$,  $\tau_{zy}\,=\displaystyle{\lim_{\Delta A \to 0}}\frac{\Delta F_y}{\Delta A}$

So, stresses are generally expressed like below:

![useful image](https://raw.githubusercontent.com/brandonkim12/brandonkim12.github.io/master/assets/mechanics_of_materials/fig_5.JPG)

<center>Fig.5 - General expressions of stresses</center>



<center>-5. Premise: the condition of material which we're getting to analyze</center>

* Homogeneous: the property of material which has the same physical and mechanical properties throughout its volume

* Isotropic: the property of material which has the same properties in all directions, then when the load P is applied to the bar through the centroid of its cross-sectional area, the bar will deform uniformly throughout the central region of its length.

  Note: Anisotropic material:  have different properties in different directions / however it also deform uniformly when subjected to the axial load P.

  ![useful image](https://raw.githubusercontent.com/brandonkim12/brandonkim12.github.io/master/assets/mechanics_of_materials/fig_8.JPG)

<center>Fig. 6 - Uniform deformation of homogeneous and isotropic material</center>

<center>-6. Average Normal Stress</center>

* if a bar is taken and divided into the large number of infinitesimally small specimen, it has been undergone uniform deformation, and it means directly that the cross section be subjected to a constant normal stress distribution just like [Fig. 7.]  

![useful image](https://raw.githubusercontent.com/brandonkim12/brandonkim12.github.io/master/assets/mechanics_of_materials/fig_9.JPG)

<center>Fig. 7 - Infinitesimally small specimen - </center>

* Each small area $\Delta\,A$ on the cross section is subjected to a force $\Delta N\,=\,\sigma\,\Delta\,A$, [Fig. 8.], and the sum of these forces acting over the entire cross-sectional area must be equivalent to the internal resultant force $\mathbb{P}$ at the section. If we let $\Delta N\,\rightarrow\sigma\,dA$ and therefore $\Delta N\,\rightarrow dN $, then, recognizing $\sigma$ is constant, we have

![useful image](https://raw.githubusercontent.com/brandonkim12/brandonkim12.github.io/master/assets/mechanics_of_materials/fig_10.JPG)

<center>Fig. 8 - Average Normal Stress</center>

$$\begin{align}+\uparrow F_{R_z}\,=\,\sum F_z ; &\,\,\,\,\, \int\,dN\,=\,\int_A \sigma\,dA \\ &N\,=\,\sigma\,A \\ & \sigma\,=\frac{N}{A}\end{align}$$

$\sigma$: average normal stress at any point on the cross-sectional area

$N$: internal resultant normal force

$A$: cross-sectional area of the bar where $\sigma$ is determined

* The stress distribution in Fig. 1–12 indicates that only a normal stress exists on any small volume element of material located at each point on the cross section. so we get the formula:
  $$\begin{align}\sum F_z\,=\,0; & \,\,\,\,\,\,\,\sigma(\Delta A)\,-\,\sigma'(\Delta A)\,=0 \\ & \sigma\,=\,\sigma' \end{align}$$

![useful image](https://raw.githubusercontent.com/brandonkim12/brandonkim12.github.io/master/assets/mechanics_of_materials/fig_11.JPG)

<center>Fig. 9 - Internal Equilibrium</center>

* It says that the normal stress components on the element must be equal in magnitude but opposite in direction. // this is based on the assumption that the material is subjected to ==uniaxial stress== and by this analysis the component is determined whether is subjected to the tension or compression.



<center>7. Average Shear Stress</center>





- References

R.C. Hibbeler, "Mechanics of materials",  Pearson, 10th ed., ch.1

