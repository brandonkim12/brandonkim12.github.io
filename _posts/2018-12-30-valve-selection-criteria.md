---
layout: post
title: 2) Valve Selection Criteria
date:  2018-12-30 23:00:00 +0900
categories:
- Engineering - Valves
feature_image: https://www.facebook.com/photo.php?fbid=1893189787425704&set=a.1893187554092594&type=3&theater
---



<center>1. Valve Coefficient</center>

When you design the pneumatic or hydraulic system, according to the Bernoulli's equation in compressible flow situation

$$gh + \frac{1}{2}v^2 + \frac{\int dP}{\rho}=const. \tag{2.1}$$ 

where $g​$ is the gravity acceleration constant, $h​$ is the height of the fluid line from the reference point, $\rho​$ is the density property of fluid being analyzed, and $\int dP​$ is the pressure drop within the measurement time scope. Above term is the mechanical energy of the fluid per unit mass. 

Usually the closure element, such as a plug or a disk, is located just off the seat, which leads to the possibility of creating a high pressure drop and faster velocities—causing cavitation, flashing, or erosion of the trim parts. In addition, if the closure element is closure to the seat and the operator is not strong enough to hold that position, it may be sucked into the seat. This problem is appropriately called *the bathtub stopper effect*. That's why we have to focus in the $\int dP$. 

In many occasion, we can approximate the $\int dP$ into $\Delta P$. As we can see in $(2.1)$,  the pressure drop is very important when you design the pneumatic or hydraulic system, because velocity of the fluid varies with the pressure drop by the valve structure*(installed flow characteristic)*, regardless of whether the height difference could be ignored (height can be measured easily). Considering that, the valve coefficients are to evaluate the performance of the valve according to the pressure drop.

$$C_v\,=Q \sqrt{\frac{S_g}{\Delta P}} \tag{2.2}$$

where $C_v\,=\,$ required flow coefficient for the valve

​              $Q\,=$ flow rate [gal/min]

​             $S_g\,=$ specific gravity of the fluid

​           $\Delta P\,=$ pressure drop [psi]

when you design the pneumatic or hydraulic system, you would often design with the  Imperial units, so we should be used to take the imperial units system. 



<center>2. Theoretical Background</center>

Let use the HGL(Hydraulic Grade Line) and EGL(Energy Grade Line) to visualize the Bernoulli's equation much easier to understand $(2.2)​$. To do this, Divide $(2.1)​$ by $g​$. Then we can evaluate

$$\underset{(along\,a\,streamline)}{\underset{Pressure\,Head}{\underline{\frac{P}{\rho g}}}+\underset{Velocity\,Head}{\underline{\frac{V^2}{2g}}}+\underset{Elevation\,Head}{\underline{h}}=\underset{Total\,Head}{\underline{H}}} \tag{2.3}$$ 



[Following contents would be the effect of inlet or outlet - fluid mechanics or the main book]

> This is the incomplete article. 





- References

1. Valve Handbook, 2nd ed., p.1.
2. Renteln P. - Manifolds, Tensors, and Forms_ An Introduction for Mathematicians and Physicists
3. Pavel Grinfeld, Tensor analysis