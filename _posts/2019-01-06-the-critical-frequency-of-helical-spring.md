---
layout: post
title: The critical frequency of the helical spring
date:  2019-01-06 20:30:00 +0900
categories:
- Engineering - Miscellaneous
feature_image: https://www.facebook.com/photo.php?fbid=1893189787425704&set=a.1893187554092594&type=3&theater
---



The governing equation for the translational vibration of the spring placed between two flat and parallel plates is

$$\frac{{\partial}^2 u}{\partial x^2}=\frac{1}{c^2}\frac{{\partial}^2 u}{\partial t^2}\tag{1}$$

$$\text{where}\begin{cases} c: & \frac{T_0}{\rho (x)} \\ T_0: & \text{The initial tension acting on the spring}\\ u: & \text{Motion of any particle at distance x}\end{cases}$$

Assume that $\rho$ is constant for any x, which means that the spring is homogeneous, we get

$$\rho=\frac{m}{l}=\frac{W}{gl},\,T_0=kl$$

$$\text{where}\begin{cases} \rho: & \text{The linear density of spring} \\ g: & \text{The gravity constant}≒9.802 m/s^2 \\ l: & \text{The length of the spring} \end{cases}$$

Then, $c^2=\frac{kgl^2}{W}$, so (1) becomes

$$\frac{{\partial}^2 u}{\partial x^2}=\frac{W}{kgl^2}\frac{{\partial}^2 u}{\partial t^2}\tag{2}$$

By the separation of the variable, we get from the equation

$$\begin{aligned}u(x,t)=X(x)T(t) \\ \frac{X''}{X}= \frac{T''}{c^2 T}=-\lambda_n \end{aligned}$$

where $\lambda_n$ means that X and T are the periodic functions. By the normal Strum-Liouville problem, we get the $\lambda_n = \frac{n^2 \pi^2}{l^2}$, So $u(x,t)$ with $X(x)$ and $T(t)$ is represented to

$$u(x,t)\,=\,\sum_{n=1}^{\infty}\sin \frac{n\pi x}{l}[A_n \cos \frac{n\pi ct}{l} + B_n\sin \frac{n \pi ct}{l}] \tag{3} $$

We call the natural frequency $w_n=\frac{n\pi c}{l}$, so replace $c$ with $\sqrt{\frac{kgl^2}{W}}$ we get $w_n=\frac{n\pi}{l}\sqrt{\frac{kgl^2}{W}}=n\pi \sqrt{\frac{kg}{W}}$.



* References
  * A First Course in Partial Differential Equations with complex variables and transform methods - H. Wein, ch.1
  * Shigley's Mechanical Engineering Design, 8th ed.
