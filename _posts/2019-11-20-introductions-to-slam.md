---
layout: post
title: 1) Introduction to SLAM
date:  2019-11-20 23:00:00 +0900
categories:
- Engineering - SLAM
feature_image: https://www.facebook.com/photo.php?fbid=1893189787425704&set=a.1893187554092594&type=3&theater
---

<center>1. What is SLAM?</center>
In robotics, SLAM(Simultaneous Localization And Mapping) means the process where a mobile robot 
1) builds a map of an unknown environment 
2) while at the same time being localizaed relative to this map. 

To localize the position, the information of surrounding is essential. However, to make a map around robot obtained by itself, there should be a knowledge about the accurate location. Therefore these problem is indispensable. SLAM performs simultaneously both mapping and position estimation to solve this kind of a problem.

![useful image](https://raw.githubusercontent.com/brandonkim12/brandonkim12.github.io/master/assets/robotics/fig_1.jpg)

<center>[Fig 1. The essential SLAM problem. A simultaneous estimate of both robot and landmark locations is required. The true locations are never known or measured directly. Observations are made between true robot and landmark locations.]</center>
<center>2. Formulation and Structure of the SLAM Problem</center>

SLAM is a process by which a mobile robot can build a map of an environment and at the same time use this map to deduce its location. In SLAM, both the trajectory of the platform and the location of all landmarks are estimated online without the need for any a priori knowledge of location.

- Preliminaries

$\textbf{x}_k:$ the state vector describing the location and orientation of the vehicle

$\textbf{u}_k:$ the control vector, applied at time $k−1$ to drive the vehicle to a state $\textbf{x}_k$ at time $k$

$\textbf{m}_i:$ a vector describing the location of the $i$th landmark whose true location is assumed time invariant

$\textbf{z}_{ik}:$ an observation taken from the vehicle of the location of the ith landmark at time $k$. When there
are multiple landmark observations at any one time or when the specific landmark is not relevant to the discussion, the observation will be written simply as $\textbf{z}_k$ .

In addition, the following sets are also defined:

$$\textbf{X}_{0:k} = ({\textbf{x}_0 , \textbf{x}_1, \dots , \textbf{x}_k}) = ({\textbf{X}_{0:k-1},\textbf{x}_k }):$$ the history of robot/vehicle locations

$$\textbf{U}_{0:k} = ({\textbf{u}_1 , \textbf{u}_2, \dots , \textbf{u}_k}) = ({\textbf{X}_{0:k-1},\textbf{x}_k }): $$ the history of control input

$\textbf{m} = ({\textbf{m}_1 , \textbf{m}_2, \dots , \textbf{m}_n}):$  the set of all landmarks

$$\textbf{Z}_{0:k} = ({\textbf{z}_1 , \textbf{z}_2, \dots , \textbf{z}_k}) = ({\textbf{Z}_{0:k-1},\textbf{z}_k }):$$ the set of all landmark observations.

