---
layout: post
title: 1) The basic of linear algebra (1) - what is the linear algebra?
date:  2018-12-23 18:00:00 +0900
categories:
- Mathematics - Linear Algebra
feature_image: https://www.facebook.com/photo.php?fbid=1893189787425704&set=a.1893187554092594&type=3&theater
---

<center>1. Origin of the linear algebra</center>

There is the historical fact that in china, the equivalent procedure for the *gauss elimination* is used as early as 200 BC. The main use of the linear algebra is to solve the **simultaneous equation system**. In *Nine Chapters of the Mathematical Art* (九章算術), whose early version of this book was burnt by the emperor Ch’in Shih Huang. In Chapter 8, there are 18 problems, all of which correspond to linear systems with between two and six unknown quantities. With one exception, all of the problems have a unique solution with the number of constraints (equations) equaling the number of unknown quantities. The first problem is:

> Now given 3 bundles of top grade paddy, 2 bundles of medium grade paddy,
> [and] 1 bundle of low grade paddy. Yield: 39 dou of grain. 2 bundles of top grade
> paddy, 3 bundles of medium grade paddy, [and] 1 bundle of low grade paddy,
> yield 34 dou. 1 bundle of top grade paddy, 2 bundles of medium grade paddy,
> [and] 3 bundles of low grade paddy, yield 26 dou. Tell: how much paddy does
> one bundle of each grade yield. [21, p. 399]

The brief information for this problem is that the paddy is grain, and the dou is a unit used for measuring volume. Interpreting this into more easier things, it is expressed like: “A combination of 3 bundles of high-quality grain, 2 bundles of medium-quality grain, and 1 bundle of low-quality grain will yield 39 barrels of flour.” The solution is like below: 

![useful image](https://raw.githubusercontent.com/brandonkim12/brandonkim12.github.io/master/assets/mathematics/fig_1.JPG)

<center>Fig. 1. Solution for the first problem in ch.8 of Nine Chapters of the Mathematical Art</center>

Let's solve this along the solution expressed above. 

$$\begin{bmatrix}1 & 2 & 3 \\ 2 & 3 & 2 \\ 3 & 1 & 1 \\ 26 & 34 & 39 \end{bmatrix}$$

Seeing [Fig. 1. (a)]. When 3rd column is subtracted from 2nd column, we get a column vector 

$$\begin{bmatrix}1 \\ -1 \\ 0 \\ 5 \end{bmatrix}$$

By subtracting this from 2nd column, we can get [Fig. 1. (b).] Getting through the process like this, we can get [Fig. 1. (c)]. Surprisingly, these processes assemble with *Gauss elimination*.



<center>2. What would we study in linear algebra?</center>

* Matrices and gauss elimination

  Like we've seen above, linear algebra starts from this kind of simple iteration to solve the systems of linear equation. The iteration is called to **Gauss elimination**, which is the method that  To make this calculations regularly expressed, we use something - matrix. Don't know? It is 

  $$\begin{bmatrix}1 & 2 & 3 \\ 2 & 3 & 2 \\ 3 & 1 & 1 \\ 26 & 34 & 39 \end{bmatrix}$$ 

  Yes, we saw it above already. This is **matrix**.

* Systems of Linear Equations, Vectors and Vector Spaces

  In section 1, we solved a bunch of equations with elimination method. this *a bunch of linear equation* is the **System of linear equations.** **Vector** is a part of the matrix in row or column sense: 

  $$\begin{bmatrix}1 \\ -1 \\ 0 \\ 5 \end{bmatrix}$$

  is the column vector. To be involved with general cases, such as representations with a bunch of variables in $\mathbb{R}$, a set of real numbers, or $\mathbb{C}$, a set of complex numbers.  **Vector space** is for this generalization. 

* Orthogonality

  The vector space is represented with independent vectors each other, then how can we define this independency? **Orthogonality** Works for the definition of independency. For example, from the coordinates system - The most common case : $xy$-coordinates -, x, y is *orthogonal*. 

* Determinants

  Generalized systems of equations, we get solution of it by the inverse matrix. If the systems of equation is represented like $\mathbb{A} \mathbb{x}\,=\,\mathbb{b}$, then $\mathbb{x}$ is found by $\mathbb{x}\,=\,\mathbb{A}^{-1}\mathbb{b}$.  to find $\mathbb{A}^{-1}$, **Determinant** is used.  The determinant is used to find out what the solution $\mathbb{x}$ is, and its applications are all around the engineering and science.

* Eigenvalues and eigenvectors

  Since now, we have briefly seen about how the solution of *system of linear equations* have been changed, from simple subtraction to more general method, using *inverse matrix*. We would just talk about more improved method to find the solution with **Eigenvalues** and their pair, **Eigenvectors**. Although it is the more complicated job to find the eigenvalues and eigenvectors rather than just find the inverse matrix, it has many advantages for engineering and science problem. we'll see.





* References

1. Christine Andrews-Larson, Roots of Linear Algebra: An Historical Exploration of Linear Systems
2. Robert A. Beezer, A First Course In Linear Algebra
3. Gilbert Strang, 3th ed., Linear Algebra and Its Applications
