---
layout: post
title: 4) The basic of tensor algebra (1) - Vector revisited
date:  2018-12-23 18:00:00 +0900
categories:
- Mathematics - Tensor Calculus
feature_image: https://www.facebook.com/photo.php?fbid=1893189787425704&set=a.1893187554092594&type=3&theater
---

Tensor is, simply speaking, the **expansion of vector**.  More strictly speaking, **The tensor inherits the property of the vector**, because the tensor is *the superordinate concept of the vector*. Once we took the subject of this article as 'vector revisited', let us start from the notion of the vector space. Wait, ***What is the vector***, then?

> Vector is the quantity which has the direction and magnitude.

Normally, many of us got the concept of the vector like above, and when you want to calculate the addition or subtraction, we often use both graphical method or arithmetic method. Firstly, the graphical method is stated below:

![useful image](https://raw.githubusercontent.com/brandonkim12/brandonkim12.github.io/master/assets/mathematics/fig_2.JPG)

<center>Fig. 1 - Graphical method for vector calculation</center>

We may think that there are some axiomatic statements to make this valid. Yes, here they are. Now we look at the axioms, definitions, and theorems for vector arithmetics.

 1.Notion of the vector space

**Definition 4.1.** A vector space is a set of $\mathbb{V}$ of elements called vectors satisfying the following axioms.

| Axiom of addition                                            | Axiom of multiplication                                      |
| ------------------------------------------------------------ | ------------------------------------------------------------ |
| $\mathbb{(x+y)+z}\,=\,\mathbb{x+(y+z)}$                      | $\alpha(\beta \mathbb{x})\,=\,(\alpha \beta)\mathbb{x}$      |
| $\mathbb{x} + \mathbb{y}\,=\,\mathbb{y} + \mathbb{x}$        | $\mathbb{1 x}\,=\,\mathbb{x}$                                |
| $\mathbb{0+x}\,=\mathbb{x+0}\,=\mathbb{x}$, $\forall \mathbb{x} \in \mathbb{V}$ | $\alpha(\mathbb{x+y})\,=\alpha\mathbb{x}\,+\alpha\mathbb{y}$ |
| $\mathbb{x+(-x)}\,=\mathbb{x-x}\,=\mathbb{0}$                | $(\alpha+\beta)x\,=\,\alpha\mathbb{x}+\beta\mathbb{x}$       |
| where $\mathbb{x}$,  $\mathbb{y}$ $\in$ $\mathbb{V}$         | $\forall \alpha,\,\beta\,\in\,\mathbb{R},\,\forall \mathbb{x},\,\mathbb{y}\,\in\,\mathbb{V}$ |

 2.Basis and Dimension of the Vector Space

Based on the arithmetic of the vector, we can set another properties of vectors: basis and dimension.

**Definition 4.2.** A set of vectors $\mathbb{x_1,\,\,x_2,\,\cdots\,x_n}​$ is called *linearly independent if there exists a set of corresponding scalars* ${\alpha}_1,\,{\alpha}_2,\,\cdots,\,{\alpha}_n\,\in\,\mathbb{R}​$, not all zero, such that

$$\sum_{i=1}^{n}\alpha_i\,\mathbb{x}_i\,=\,0 \tag{4.1}$$

Otherwise, $\mathbb{x}_i\,(i\,=1,2,\cdots,n)$ are called linearly independent.

**Definition 4.3.** The vector

$\mathbb{x}\,=\,\sum_{i=1}^{n} \alpha_i\mathbb{x}_i\tag{4.2}$

is called linear combination of the vectors $\mathbb{x}_i\,(i\,=1,2,\cdots,n)$ where $\alpha_i\in\mathbb{R}\, (i\,=1,2,\cdots,n)$

***Theorem 4.1.*** The set of n non-zero vectors $\mathbb{x}_i\,(i\,=1,2,\cdots,n)$ is linearly dependent if and only if some vector $\mathbb{x}_k\,(2≤k≤n)$ is a linear combination of the preceding ones $\mathbb{x}_j\,(j\,=1,2,\cdots,k-1)$.

*proof*. if the vectors $$\mathbb{x}_i\,(i\,=1,2,\cdots,n)$$ are linearly independent, then $\sum_{i=1} ^n \alpha_i\mathbb{x}_i=0$  where not all $\alpha_i=0\,(i=k+1,\cdots,n)$. Then,

$$\sum_{i=1}^k \alpha_i \mathbb{x}_i\,=\,\mathbb{0}\,\Rightarrow\,\mathbb{x}_k=\sum_{i=1}^{k-1}\frac{-\alpha_i}{\alpha_k}\mathbb{x}_i$$

By this, the case $k=1\,\Rightarrow \alpha_1 \mathbb{x}_1=\mathbb{0} \Rightarrow \mathbb{x}_1=\mathbb{0}$. Thus, the sufficiency is proved, while the necessity is evident.

**Definition 4.4.**  A basis of a vector space $\mathbb{V}$ is a set $\mathbb{G}$ of linearly independent vectors such that every vector in $\mathbb{V}$ is a linear combination of elements of $\mathbb{G}$. A vector space $\mathbb{V}$ is finite-dimensional if it has a finite basis.

In Engineering and physics, infinite basis doesn't express the actual situation. For this reason, we only take the finite basis for $\mathbb{V}$. 

***Theorem 4.2.*** All the bases of a finite-dimensional vector space $\mathbb{V}$ contain the same number of vectors.

*Proof*. Let $$\mathbb{G} = \begin{Bmatrix}g_1, g_2,\cdots, g_n \end{Bmatrix}$$ and $$\mathbb{F} = \begin{Bmatrix}f_1, f_2, \cdots , f_m\end{Bmatrix}$$ be two arbitrary bases of $\mathbb{V}$ with different numbers of elements, say $m >n$. Then, every vector in $\mathbb{V}$ is a linear combination of the following vectors:

$$\begin{Bmatrix}f_1, g_1, g_2, \cdots , g_n. \end{Bmatrix}\tag{4.3}$$

These vectors are non-zero and linearly dependent. Thus, according to Theorem 4.1 we can find such a vector $g_k$, which is a linear combination of the preceding ones. Excluding this vector we obtain the set $\mathbb{G}'$ by

$$\begin{Bmatrix}f_1, g_1, g_2, \cdots , g_{k−1}, g_{k+1}, . . . , g_n\end{Bmatrix}$$

again with the property that every vector in $\mathbb{V}$ is a linear combination of the elements of $\mathbb{G}'$. Now, we consider the following vectors

$$\begin{Bmatrix}f_1, f_2, g_1, g_2, \cdots , g_{k−1}, g_{k+1}, . . . , g_n\end{Bmatrix}$$

and repeat the excluding procedure just as before. We see that none of the vectors fi can be eliminated in this way because they are linearly independent. As soon as all $g_i (i = 1, 2, . . ., n)$ are exhausted we conclude that the vectors

$$\begin{Bmatrix}f_1, f_2, . . . , f_{n+1}\end{Bmatrix}$$

are linearly dependent. This contradicts, however, the previous assumption that they belong to the basis $\mathbb{F}$.

**Definition 4.5.** The dimension of a finite-dimensional vector space $\mathbb{V}$ is the number of elements in a basis of $\mathbb{V}$.

***Theorem 4.3.*** Every set $\mathbb{F} = \begin{Bmatrix}f_1, f_2, \cdots , f_n\end{Bmatrix}$ of linearly independent vectors in an n-dimensional vectors space $\mathbb{V}$ forms a basis of $\mathbb{V}$. Every set of more than n vectors is linearly dependent.

*proof*. The process is just same to that of ***Theorem 4.2.***, so the process can be skipped.

***Theorem 4.4.*** Every set $\mathbb{F} = \begin{Bmatrix}f_1, f_2, \cdots , f_m\end{Bmatrix}$ of linearly independent vectors in an n-dimensional vector space V can be extended to a basis.

*Proof.* If $m = n$, then $\mathbb{F}$ is already a basis according to ***Theorem 4.3.*** If $m < n$, then we try to find $n − m$ vectors $f_{m+1}, f_{m+2}, \cdots , f_n$, such that all the vectors $f_i$, that is, $f_1, f_2, . . . , f_m, f_{m+1}, . . . , f_n$ are linearly independent and consequently form a basis. Let us assume, on the contrary, that only $k < n− m$ such vectors can be found. In this case, for all $x \in \mathbb{V}$ there exist scalars $\alpha, \alpha_1, \alpha_2, . . ., \alpha_{m+k}$, not all zero, such that

$$\alpha_x + \alpha_1f_1 + \alpha_2f_2 + . . . + \alpha_{m+k}f_{m+k} = 0,$$

where $α \neq 0$ since otherwise the vectors $f_i (i = 1, 2, . . .,m + k)$ would be linearly dependent. Thus, all the vectors x of V are linear combinations of $f_i (i = 1, 2, . . .,m + k).$ Then, the dimension of $\mathbb{V}$ is $m +k < n,$ which contradicts the assumption of this theorem.




* References

1. Itskov M., Tensor Algebra and Tensor Analysis for Engineers
2. Renteln P. - Manifolds, Tensors, and Forms_ An Introduction for Mathematicians and Physicists
3. Pavel Grinfeld, Tensor analysis

