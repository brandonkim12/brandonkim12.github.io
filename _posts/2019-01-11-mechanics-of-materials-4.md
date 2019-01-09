---
layout: post
title: 4) Mechanical Properties of Materials - Axial Load
date:  2019-01-11 23:30:00 +0900
categories:
- Engineering - Mechanics of Materials
feature_image: https://www.facebook.com/photo.php?fbid=1893189787425704&set=a.1893187554092594&type=3&theater
---

<center>1. Saint-Venant's Principle - The First Sssumptions from The Theory of Elasticity</center>

We have shown that the mathematical relationship between stress and strain depends on the type of material from which the body is made. In particular, if the material behaves in a linear elastic manner, then Hooke’s law applies, and there is a proportional relationship between stress and strain. Using this idea, consider the manner in which a rectangular bar will deform elastically when the bar is subjected to the force P applied along its centroidal axis, [Fig. 4.1].

![useful image](https://raw.githubusercontent.com/brandonkim12/brandonkim12.github.io/master/assets/mechanics_of_materials/fig_33.JPG)

<center>Fig. 4.1. Figure to state the saint-venant's principle</center>

If the material remains elastic, then the strains caused by this deformation are directly related to the stress in the bar through Hooke’s law, $\sigma = E\epsilon$. As a result, a profile of the variation of the stress distribution acting at sections a–a, b–b, and c–c, will look like that shown in [Fig. 4.2.].

![useful image](https://raw.githubusercontent.com/brandonkim12/brandonkim12.github.io/master/assets/mechanics_of_materials/fig_34.JPG)

<center>Fig. 4.2. Description of stress-behaviors at each section</center>

By comparison, the stress tends to reach *a uniform value* at **section c–c**, which is sufficiently removed from the end since the localized deformation caused by P vanishes. *The minimum distance from the bar’s end where this occurs can be determined using a mathematical analysis based on the theory of elasticity.* It has been found that this distance should at least be equal to the largest dimension of the loaded cross section. (It would be stated in the theory of elasticity in detail.) Hence, **section c–c should be located at a distance at least equal to the width (not the thickness) of the bar, and our interests are almost in this region, c-c.** This fact is *The Saint-Venant's Principle.*

<br>

<center>2. Eleastic Deformation of an Axially Loaded Member</center>

$$\sigma=\frac{N(x)}{A(x)} \text{ and }\epsilon=\frac{d\delta}{dx}$$

When the stress doesn't exceed the elastic limit, we can apply the Hooke's law: $\sigma = E(x) \epsilon$, and by this we can obtain

$$\begin{matrix}\frac{N(x)}{A(x)}\,=\,E(x)\frac{d\delta}{dx} \\ d\delta\,=\,\frac{N(x)dx}{A(x)E(x)}\\ \delta\,=\,\int_0^L\frac{N(x)dx}{A(x)E(x)}\end{matrix} \tag{4.1.}$$

$$\text{where}\begin{cases}\delta =& \text{displacement of one point} \\ & \text{on the bar relative to the other point} \\ L = & \text{original length of bar} \\ N(x) = & \text{internal axial force at the section,} \\ & \text{located a distance x from one end} \\ A(x) = & \text{cross-sectional area of the bar} \\ & \text{expressed as a function of x} \\ E(x)= & \text{modulus of elasticity for the material} \\ & \text{expressed as a function of x} \end{cases}$$

In constant load and cross-sectional area situation, which is the 'Engineering Situation' as we've seen in 'conventional stress-strain curve', we can take $N(x),\,A(x),\,E(x)$ as all constant. Then, (4.1.) is to be

$$\delta\,=\,\sum\frac{NL}{EA} \tag{4.2.}$$

When the material is elongated, sign is (+), otherwise (-). This is *the sign convention about the axial deformation.* As we assumed that *we analyze the deformation in c-c region, which means that the deformation is linear when the material is not in the plastic deformation region,* we can apply the principle of superposition.



![useful image](https://raw.githubusercontent.com/brandonkim12/brandonkim12.github.io/master/assets/mechanics_of_materials/fig_35.JPG)



> This is not a complete article, so please take this in your mind.
>

* References
  * R.C. Hibbeler, "Mechanics of materials",  Pearson, 10th ed., ch.4
  * Ferdinand P. Beer, Mechanics of Materials, 5th ed., ch.3
