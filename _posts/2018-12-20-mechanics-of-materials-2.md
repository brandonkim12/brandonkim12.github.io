---
layout: post
title: 2) Stress and Strain - Strain
date:  2018-12-20 23:30:00 +0900
categories:
- Engineering - Mechanics of Materials
feature_image: https://www.facebook.com/photo.php?fbid=1893189787425704&set=a.1893187554092594&type=3&theater
---

<center>1. Deformation and Strain</center>

When a excessive stress is applied to the body of certain material, the shape of the body would be changed. It is called to **Deformation**. The deformation includes the case of yielding, neckling, and rupture, etc., but in this chapter yielding is the principal subject. In a general sense, <u>the deformation will not be uniform throughout the body</u>, and so the change in geometry of any line segment within the body may vary substantially along its length. So, normally the deformation is measured for a small specimen of a certain material.

![useful image](https://raw.githubusercontent.com/brandonkim12/brandonkim12.github.io/master/assets/mechanics_of_materials/fig_15.JPG)

<center>Fig.1 - The specimen for yielding experiment</center>

But also one can realize that the deformation depends on the orientation of the specimen at the point. Looking the [Fig. 2], the vertical line is lengthened, the horizontal line is shortened, and the inclined line changes its length and rotates. 

![useful image](https://raw.githubusercontent.com/brandonkim12/brandonkim12.github.io/master/assets/mechanics_of_materials/fig_16.JPG)

<center>Fig. 2 - Line representation in process of yielding experiment</center>



<center>2. The Normal Strain and Shear Strain</center>

Strain is measured along the **Normal direction**, Normal force for the reference surface, and **Transverse direction**, Transverse force for the reference surface. 

Firstly, **Normal Strain** $\epsilon$ is expressed as $\epsilon\,=\,\frac{L_0\,-\,L_f}{L_0}$, which $L_0$: Initial length of the specimen, $L_f$: final length of the specimen. 

![useful image](https://raw.githubusercontent.com/brandonkim12/brandonkim12.github.io/master/assets/mechanics_of_materials/fig_17.JPG)

<center>Fig. 3. - The abstract diagram of actual tension experiment</center>

In a practical experiment like [Fig. 2] and [Fig.3], $\Delta s$ would be changed into $\Delta s'$ if the force P exerted on the body of specimen. In this case, the strain is expressed like $\epsilon\,=\,\underset{\Delta s \rightarrow 0}{\lim}\frac{\Delta s'\,=\,\Delta s}{\Delta s}$. Since the unit of numerator and denominator is the same, **The strain is the non-dimensional value.** Although the strain has no dimension, the unit of the strain is often expressed as [$\mu m/\mu m$]for convenience. 

![useful image](https://raw.githubusercontent.com/brandonkim12/brandonkim12.github.io/master/assets/mechanics_of_materials/fig_18.JPG)

<center>Fig. 4. - Deformed element</center>

Secondly, **Shear strain** $\gamma$ is expressed as $\gamma \,=\,\frac{\pi}{2}-\theta$ for [Fig. 4].

What one can see in [Fig. 4] is, the **normal strain** is changed into

$$\begin{matrix}(1+\epsilon_x)\Delta x & (1+\epsilon_y)\Delta y & (1+\epsilon_x)\Delta z \end{matrix}$$

which makes *a change of volume of the element.* and the **Shear strain** is changed into

$$\begin{matrix}\frac{\pi}{2}-\gamma_{xy} & \frac{\pi}{2}-\gamma_{yz} & \frac{\pi}{2}-\gamma_{xz} \end{matrix}$$

which makes a *change in the shape of the element.*



* References
  * R.C. Hibbeler, "Mechanics of materials",  Pearson, 10th ed., ch.2
  * Ferdinand P. Beer, Mechanics of Materials, 5th ed., ch.2