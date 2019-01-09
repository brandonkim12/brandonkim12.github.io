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

By comparison, the stress tends to reach *a uniform value* at **section c–c**, which is sufficiently removed from the end since the localized deformation caused by P vanishes. *The minimum distance from the bar’s end where this occurs can be determined using a mathematical analysis based on the theory of elasticity.* It has been found that this distance should at least be equal to the largest dimension of the loaded cross section. (It would be stated in the theory of elasticity in detail.) Hence, **section c–c should be located at a distance at least equal to the width (not the thickness) of the bar, and our interests are almost in this region, c-c.** This fact is *Te Saint-Venant's Principle.*

<br>

<center>2. Eleastic Deformation of an Axially Loaded Member</center>

![useful image](https://raw.githubusercontent.com/brandonkim12/brandonkim12.github.io/master/assets/mechanics_of_materials/fig_36.JPG)

<center>Fig. 4.3. General Situation of Elastic Deformation</center>

Think about the general situation of elastic deformation. What we want to know is $\delta$, the infinitesimal length changed by $P_1$ and $P_2$. But wait, how can we find $P_1$ and $P_2$? To make this difficulty up, we get a infinitesimal element.

![useful image](https://raw.githubusercontent.com/brandonkim12/brandonkim12.github.io/master/assets/mechanics_of_materials/fig_37.JPG)

<center>Fig. 4.4. Infinitesimal Element to Calculate the δ Out</center>

The resultant internal axial force will be a function of x since the external distributed loading will cause it to vary along the length of the bar. Now we take $P_1$ and $P_2$ place with $N(x)$, and then from this we can start.

$$\sigma=\frac{N(x)}{A(x)} \text{ and }\epsilon=\frac{d\delta}{dx}$$

When the stress doesn't exceed the elastic limit, we can apply the Hooke's law: $\sigma = E(x) \epsilon$, and by this we can obtain

$$\begin{matrix}\frac{N(x)}{A(x)}\,=\,E(x)\frac{d\delta}{dx} \\ d\delta\,=\,\frac{N(x)dx}{A(x)E(x)}\\ \delta\,=\,\int_0^L\frac{N(x)dx}{A(x)E(x)}\end{matrix} \tag{4.1.}$$

$$\text{where}\begin{cases}\delta =& \text{displacement of one point} \\ & \text{on the bar relative to the other point} \\ L = & \text{original length of bar} \\ N(x) = & \text{internal axial force at the section,} \\ & \text{located a distance x from one end} \\ A(x) = & \text{cross-sectional area of the bar} \\ & \text{expressed as a function of x} \\ E(x)= & \text{modulus of elasticity for the material} \\ & \text{expressed as a function of x} \end{cases}$$

In constant load and cross-sectional area situation, which is the 'Engineering Situation' as we've seen in 'conventional stress-strain curve', we can take $N(x),\,A(x),\,E(x)$ as all constant. Then, (4.1.) is to be

$$\delta\,=\,\sum\frac{NL}{EA} \tag{4.2.}$$

When the material is elongated, sign is (+), otherwise (-). This is *the sign convention about the axial deformation.* As we assumed that *we analyze the deformation in c-c region, which means that the deformation is linear when the material is not in the plastic deformation region,* we can apply the principle of superposition. The following two conditions must be satisfied if the principle of superposition is to be applied.

1. The loading $N$ must be linearly related to the stress $\sigma$ or displacement $\delta$ that is to be determined. For example, the equations $\sigma = \frac{N}{A}$ and $\delta = \frac{NL}{AE}$ involve a linear relationship between $\sigma$ and $N$, and $\delta$ and $N$.

  ![useful image](https://raw.githubusercontent.com/brandonkim12/brandonkim12.github.io/master/assets/mechanics_of_materials/fig_35.JPG)

  <center>Fig. 4.5. The condition which the principle of superposition is not applied</center>

2. The loading must not significantly change the original geometry or configuration of the member. If significant changes do occur, the direction and location of the applied forces and their moment arms will change. For example, consider the slender rod shown in [Fig. 4.5.], which is subjected to the load $\mathbf{P}$. In [Fig. 4.5.], $\mathbf{P}$ is replaced by two of its components, $\mathbf{P} = \mathbf{P_1} + \mathbf{P_2}$. If $\mathbf{P}$ causes the rod to deflect a large amount, as shown, the moment of this load about its support, $Pd$, will not equal the sum of the moments of its component loads, $Pd \neq P_1d_1 + P_2d_2$, because $d_1 \neq d_2 \neq d$.

<br>

<center>3. Statically Indeterminate Axially Loaded Members</center>

Remember the statics class? At that time, we took the redundant force off to find out the force acting on the certain support. Now we have to take advantage of the redundant forces to find out what the deformation of the material actually is *when the equations of equilibrium are not sufficient to determine all the reactions on a member.* In this time, commonly **the compatibility conditions specify the displacement constraints that occur at the supports or other points on a member.** Consider a example to explain the case we have to apply the compatibility to statically indeterminate problem.

![useful image](https://raw.githubusercontent.com/brandonkim12/brandonkim12.github.io/master/assets/mechanics_of_materials/fig_38.JPG)

<center>4.6. Statically Indeterminate Problem - Example</center>

How to find the force acting on A and B when 500N is acting on C downward? We take the information from picture that $\delta _{A/B} = 0$ and $F_A + F_B = 500[N]$, so let's get start with this. using a load–displacement relationship, which depends on the material behavior, we can find out the internal force in segment $AC$ is $+F_A$, and in segment $CB$ it is $-F_B$. Again, $\delta_{A/B} = 0$, which means that

$$\frac{F_A (2\text{m})}{AE}-\frac{F_B (\text{3m})}{AE}= 0$$

By this, we can get $F_A = 300N\text{ and }F_B = 200N$.text

This method of solution, which can make us solve statically indeterminate problems by writing the compatibility equation using the principle of superposition, is often referred to as the ***flexibility*** or ***force method of analysis***. The procedure for the analysis includes these kind of steps:

**Compatibility.**

* Choose one of the supports as redundant and write the equation of compatibility. To do this, the known displacement at the redundant support, which is usually zero, is equated to the displacement at the support caused only by the external loads acting on the member plus (vectorially) the displacement at this support caused only by the redundant reaction acting on the member

**Load–Displacement.**

* Express the external load and redundant displacements in terms of the loadings by using a load–displacement relationship, such as $\delta = \frac{NL}{AE}$. 

* Once established, the compatibility equation can then be solved for the magnitude of the redundant force. 

**Equilibrium.**

* Draw a free-body diagram and write the appropriate equations of equilibrium for the member using the calculated result for the redundant. Solve these equations for the other reactions.

<br>

<center>4. Thermal Stress, Stress Concentrations, Inelastic Deformation, and Residual Stress</center>

* Thermal Stress: A change in temperature can cause a body to change its dimensions. Generally, *if the temperature increases, the body will expand, whereas if the temperature decreases, it will contract.* **(1) If this is the case, (2) and the material is homogeneous and isotropic,** it has been found from experiment that the displacement of the end of a member having a length L can be calculated using the formula

$$\delta _T\,=\,\alpha \Delta TL \tag{4.2}$$

$$\text{Where }\begin{cases} \alpha: & \text{a property of the material,} \\ &  \text{referred to as the linear coefficient} \\ & \text{of thermal expansion.} \\ \Delta T: &  \text{the algebraic change in} \\ & \text{temperature of the member} \\ L: & \text{the original length of the member} \\ \delta_T: & \text{the algebraic change in the length of the member} \end{cases}$$ 

* Stress Concentrations: As we've seen on the [Fig. 4.1.], [Fig. 4.7.] states the concentration effect for the local region such as hole, crack, etc.. Consider, for example, the bar in [Fig. 4.7.a], which is subjected to an axial force N. 
  Here the once horizontal and vertical grid lines deflect into an irregular pattern around the hole centered in the bar. The maximum normal stress in the bar occurs on section a–a, since it is located at the bar’s smallest cross-sectional area. 
  Provided the material behaves in a linear elastic manner, the stress distribution acting on this section can be determined either from a mathematical analysis, using the theory of elasticity, or experimentally by measuring the strain normal to section a–a and then calculating the stress using Hooke’s law, $$\sigma = E\epsilon​$$. 



![useful image](https://raw.githubusercontent.com/brandonkim12/brandonkim12.github.io/master/assets/mechanics_of_materials/fig_39.JPG)

<center>4.7. The Diagram for The Stress Concentration: Normal Bar </center>

If instead the bar has a reduction in its cross section, using shoulder fillets as in [Fig. 4.8.a], then at the smallest cross-sectional area, section a–a, the stress distribution will look like that shown in [Fig. 4.8.b].

![useful image](https://raw.githubusercontent.com/brandonkim12/brandonkim12.github.io/master/assets/mechanics_of_materials/fig_40.JPG)

<center>4.8. The Diagram for The Stress Concentration: Reduced Bar</center>

In both of these cases, force equilibrium requires the magnitude of the resultant force developed by the stress distribution at section a–a to be equal to $N$. In other words,

$$N = \int_A \sigma dA \tag{4.3}$$

In engineering practice, above integral is hard to be defined and calculated. Instead, we have the set of the values and graph of the stress concentration factor $K$ such that $K = \frac{\sigma_{\text{max}}}{\sigma_{\text{avg}}}$.

![useful image](https://raw.githubusercontent.com/brandonkim12/brandonkim12.github.io/master/assets/mechanics_of_materials/fig_41.JPG)

<center>4.9. The Graph of Stress Concentration Factor K - Reduced Bar</center>

![useful image](https://raw.githubusercontent.com/brandonkim12/brandonkim12.github.io/master/assets/mechanics_of_materials/fig_42.JPG)

<center>4.10. The Graph of Stress Concentration Factor K - Normal Bar</center>

Using this table, we get the upper limit for the engineering design for each cases, $\sigma_{\text{max}}=K \sigma_{\text{avg}}$. 

* Inelastic Axial Deformation: 

<br>

> This is not a complete article, so please take this in your mind.
>

* References
  * R.C. Hibbeler, "Mechanics of materials",  Pearson, 10th ed., ch.4
  * Ferdinand P. Beer, Mechanics of Materials, 5th ed., ch.3
