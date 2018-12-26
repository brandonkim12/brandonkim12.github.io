---
layout: post
title: 4) The basic of tensor algebra (1) - Vector revisited
date:  2018-12-23 18:00:00 +0900
categories:
- Mathematics - Tensor Calculus
feature_image: https://www.facebook.com/photo.php?fbid=1893189787425704&set=a.1893187554092594&type=3&theater
---

Tensor is, simply speaking, the **expansion of vector**.  More strictly speaking, **The tensor inherits the property of the vector**, because the tensor is *the superordinate concept of the vector*. Once we took the subject of this article as 'vector revisited', let us start from the notion of the vector space.

 1.Notion of the vector space

**Definition 4.1.** A vector space is a set of $\mathbb{V}$ of elements called vectors satisfying the following axioms.

| Axiom of addition                                            | Axiom of multiplication                                      |
| ------------------------------------------------------------ | ------------------------------------------------------------ |
| $\mathbb{(x+y)+z}\,=\,\mathbb{x+(y+z)}$ (associative)        | $\alpha(\beta \mathbb{x})\,=\,(\alpha \beta)\mathbb{x}$ (multiplication of scalar) |
| $\mathbb{x} + \mathbb{y}\,=\,\mathbb{y} + \mathbb{x}$ (commutative) | $\mathbb{1 x}\,=\,\mathbb{x}$                                |
| $\mathbb{0+x}\,=\mathbb{x+0}\,=\mathbb{x}$, $\forall \mathbb{x} \in \mathbb{V}$ ($\mathbb{0}$: identity element) | $\alpha(\mathbb{x+y})\,=\alpha\mathbb{x}\,+\alpha\mathbb{y}$ (distributive for scalar addition) |
| $\mathbb{x+(-x)}\,=\mathbb{x-x}\,=\mathbb{0}$  ($-\mathbb{x}$: reciprocal element) | $(\alpha+\beta)x\,=\,\alpha\mathbb{x}+\beta\mathbb{x}$ (distributive for vector addition) |
| where $\mathbb{x}$,  $\mathbb{y}$ $\in$ $\mathbb{V}$         | $\forall \alpha,\,\beta\,\in\,\mathbb{R},\,\forall \mathbb{x},\,\mathbb{y}\,\in\,\mathbb{V}$ |

 2.Basis and Dimension of the Vector Space

Based on the arithmetic of the vector, we can set another properties of vectors: basis and dimension.

**Definition 4.2.** A set of vectors $\mathbb{x_1,\,\,x_2,\,\cdots\,x_n}$ is called *linearly independent if there exists a set of corresponding scalars* ${\alpha}_1,\,{\alpha}_2,\,\cdots,\,{\alpha}_n\,\in\,\mathbb{R}$, not all zero, such that

$$\sum_{i=1}^{n}\alpha_i\,\mathbb{x}_i\,=\,0 \tag{4.1}$$

​	Otherwise, $\mathbb{x}_i\,(i\,=1,2,\cdots,n)$ are called linearly independent.

***Theorem 4.1.*** The set of n non-zero vectors $\mathbb{x}_i\,(i\,=1,2,\cdots,n)$ is linearly dependent iff some vector $\mathbb{x}_k\,(2≤k≤n)$ is a linear combination of the preceding ones $\mathbb{x}_j\,(j\,=1,2,\cdots,k-1)$.



> This is not the completed documents.




* References

1. Itskov M., Tensor Algebra and Tensor Analysis for Engineers
2. Renteln P. - Manifolds, Tensors, and Forms_ An Introduction for Mathematicians and Physicists
3. Pavel Grinfeld, Tensor analysis

