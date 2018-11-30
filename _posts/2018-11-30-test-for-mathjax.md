---
layout: post
title: Test For Mathjax
date:  2018-11-30 01:58:00 +0900
categories:
- Mathematics
feature_image: https://www.facebook.com/photo.php?fbid=1893189787425704&set=a.1893187554092594&type=3&theater
---

5년 전에 해놨던 것을 그대로 가져온다. 양해 부탁드린다.
cf) 어떤 면에서 계산하는지에 대한 언급은 딱 한 번만 하겠다. 그 이후로는 모두 동일한 면에 대해서 계산한다. 

지금부터 하나의 그림을 계속 사용할텐데, 양해 부탁드린다.

1. Grad

<div class="separator" style="clear: both; text-align: center;"><a href="https://3.bp.blogspot.com/-wTEihctENx4/WkshkCwlfNI/AAAAAAAAScg/CogdBjEHbswPXYSfpLAHlhOjLI4x9EUKQCLcBGAs/s1600/Continuity%2BEquation%2B-%2BControl%2BVolume.jpg" imageanchor="1" style="margin-left: 1em; margin-right: 1em;"><img border="0" src="https://3.bp.blogspot.com/-wTEihctENx4/WkshkCwlfNI/AAAAAAAAScg/CogdBjEHbswPXYSfpLAHlhOjLI4x9EUKQCLcBGAs/s640/Continuity%2BEquation%2B-%2BControl%2BVolume.jpg" width="640" height="359" data-original-width="590" data-original-height="331" /></a></div>
어떤 함수 Φ를 정의할 때, Φ의 Gradient Grad(Φ)는 다음과 같다.
$$\nabla\phi\,\,=\,\,\lim_{\int_\,d\tau \to 0}\frac{\int_\,\phi\,d\sigma}{\int_\,d\tau}$$

원점 O에서 이것을 해석해 보자. Cartesian Coordinate 상에서 각 평면들에 대해서 ∫φdσ는 다음과 같이 나타난다.
$$\int_\,\phi\,d\sigma\,\,= $$
$$\hat{x}[-\iint_{ABCD}^{}(\phi-\frac{\partial \phi}{\partial x} \frac{dx}{2})dydz\,\,\,+\iint_{EFGH}^{}(\phi+\frac{\partial \phi}{\partial x} \frac{dx}{2})dydz]$$
$$+\,\hat{y}[-\iint_{CDHG}^{}(\phi-\frac{\partial \phi}{\partial y} \frac{dy}{2})dxdz\,\,\,+\iint_{ABEF}^{}(\phi+\frac{\partial \phi}{\partial y} \frac{dy}{2})dxdz]$$
$$+\,\hat{z}[-\iint_{ADHE}^{}(\phi-\frac{\partial \phi}{\partial z} \frac{dz}{2})dxdy\,\,\,+\iint_{BCGF}^{}(\phi+\frac{\partial \phi}{\partial z} \frac{dz}{2})dxdy]$$
$$=\,\hat{x}[\iiint_\,\frac{\partial \phi}{\partial x}dxdydz]\,+\,\hat{y}[\iiint_\,\frac{\partial \phi}{\partial y}dxdydz]+\,\hat{z}[\iiint_\,\frac{\partial \phi}{\partial z}dxdydz]$$

Infinitesimal Space에서 편도함수들의 값 변화가 거의 없기 때문에 위의 편도함수들을 상수라 근사한다. 앞으로 이런 이유에서 적분 기호를 생략하기로 한다. 따라서 아래의 결과가 도출된다.

$$\int_\,\phi\,d\sigma\,=\,\hat{x}\frac{\partial \phi}{\partial x}dxdydz\,+\,\hat{y}\frac{\partial \phi}{\partial y}dxdydz+\,\hat{z}\frac{\partial \phi}{\partial z}dxdydz$$

그리고,
$$\int_\,d\tau\,\Rightarrow\,dxdydz$$
이므로, 상기 보였듯 Grad(Φ)는
$$\nabla\phi\,\,=\,\,\lim_{\int_\,d\tau \to 0}\frac{\int_\,\phi\,d\sigma}{\int_\,d\tau}$$

2. Div



<div class="separator" style="clear: both; text-align: center;"><a href="https://3.bp.blogspot.com/-wTEihctENx4/WkshkCwlfNI/AAAAAAAAScg/CogdBjEHbswPXYSfpLAHlhOjLI4x9EUKQCLcBGAs/s1600/Continuity%2BEquation%2B-%2BControl%2BVolume.jpg" imageanchor="1" style="margin-left: 1em; margin-right: 1em;"><img border="0" src="https://3.bp.blogspot.com/-wTEihctENx4/WkshkCwlfNI/AAAAAAAAScg/CogdBjEHbswPXYSfpLAHlhOjLI4x9EUKQCLcBGAs/s640/Continuity%2BEquation%2B-%2BControl%2BVolume.jpg" width="640" height="359" data-original-width="590" data-original-height="331" /></a></div>
어떤 벡터 함수 V를 정의할 때, V의 Divergence Div(V)는 다음과 같다. $$\nabla\cdot\,\mathbb{V}\,\,=\,\,\lim_{\int_\,d\tau \to 0}\frac{\int_\,\mathbb{V}\,\cdot\,d\sigma}{\int_\,d\tau} $$
원점 O에서 이것을 해석해 보자. Cartesian Coordinate 상에서 각 평면들에 대해서 ∫V·dσ는 다음과 같이 나타난다.
$$\int_\,\mathbb{V}\,\cdot\,d\sigma\,\,= $$
$$-\iint_\,[(V_x-\frac{\partial V_{x}}{\partial x} \frac{dx}{2})\hat{x}\,\cdot\,dydz\hat{x}]\,\,+\iint_\,[(V_x+\frac{\partial V_{x}}{\partial x} \frac{dx}{2})\hat{x}\,\cdot\,dydz\hat{x}]$$
$$-\iint_\,[(V_y-\frac{\partial V_{y}}{\partial y} \frac{dy}{2})\hat{y}\,\cdot\,dxdz\hat{y}]\,\,+\iint_\,[(V_y+\frac{\partial V_{y}}{\partial y} \frac{dy}{2})\hat{y}\,\cdot\,dxdz\hat{y}]$$
$$-\iint_\,[(V_z-\frac{\partial V_{z}}{\partial z} \frac{dz}{2})\hat{z}\,\cdot\,dxdy\hat{z}]\,\,+\iint_\,[(V_z+\frac{\partial V_{z}}{\partial z} \frac{dz}{2})\hat{z}\,\cdot\,dxdy\hat{z}]$$
$$=\int_\,(\frac{\partial V_{x}}{\partial x}+\,\,\frac{\partial V_{y}}{\partial y}+\,\,\frac{\partial V_{z}}{\partial z})\,d\,\tau$$
적분 기호를 생략하면 다음과 같다.
$$=(\frac{\partial V_{x}}{\partial x}+\,\,\frac{\partial V_{y}}{\partial y}+\,\,\frac{\partial V_{z}}{\partial z})\,d\,\tau$$
그리고,
$$\int_\,d\tau\,\Rightarrow\,dxdydz$$
이므로, 상기 보였듯 Div(V)는
$$\nabla\cdot\,\mathbb{V}\,\,=\,\,\lim_{\int_\,d\tau \to 0}\frac{\int_\,\mathbb{V}\,\cdot\,d\sigma}{\int_\,d\tau} $$</p>

3. Curl

<div class="separator" style="clear: both; text-align: center;"><a href="https://3.bp.blogspot.com/-wTEihctENx4/WkshkCwlfNI/AAAAAAAAScg/CogdBjEHbswPXYSfpLAHlhOjLI4x9EUKQCLcBGAs/s1600/Continuity%2BEquation%2B-%2BControl%2BVolume.jpg" imageanchor="1" style="margin-left: 1em; margin-right: 1em;"><img border="0" src="https://3.bp.blogspot.com/-wTEihctENx4/WkshkCwlfNI/AAAAAAAAScg/CogdBjEHbswPXYSfpLAHlhOjLI4x9EUKQCLcBGAs/s640/Continuity%2BEquation%2B-%2BControl%2BVolume.jpg" width="640" height="359" data-original-width="590" data-original-height="331" /></a></div>
어떤 벡터 함수 V를 정의할 때, V의 Curl Curl(V)는 다음과 같다.
$$\nabla\times\,\mathbb{V}\,\,=\,\,\lim_{\int_\,d\tau \to 0}\frac{\int_\,d\sigma\,\times\,\mathbb{V}}{\int_\,d\tau} $$
원점 O에서 이것을 해석해 보자. Cartesian Coordinate 상에서 각 평면들에 대해서 ∫dσXV는 다음과 같이 나타난다.
(1)
$$\Leftarrow\,\,(dx\,\,direction)$$
$$:\,-\hat{x}\int_\,d\,yd\,z\,\,\times\,\,[\int_\,(V_y-\frac{\partial V_{y}}{\partial x}\,\frac{dx}{2})\hat{y}\,+\,\int_\,(V_z\,+\frac{\partial V_{z}}{\partial x}\,\frac{dx}{2}\hat{z})] $$
$$=\,-\int_\,(V_y-\frac{\partial V_{y}}{\partial x}\,\frac{dx}{2})\,dydz\,\hat{z}\,+\,\int_\,(V_z\,+\,\frac{\partial V_z}{\partial x}\,\frac{dx}{2})\,dydz\,\hat{y} $$
$$\Rightarrow\,\,(dx\,\,direction)$$
$$=\,\int_\,(V_y+\frac{\partial V_{y}}{\partial x}\,\frac{dx}{2})\,dydz\,\hat{z}\,-\,\int_\,(V_z\,-\,\frac{\partial V_z}{\partial x}\,\frac{dx}{2})\,dydz\,\hat{y} $$
$$\therefore,\,\Leftarrow+\,\Rightarrow\,=\,\frac{\partial V_{y}}{\partial x}\,dxdydz\hat{z}-\,\frac{\partial V_{z}}{\partial x}\,dxdydz\hat{y} $$
(2) 
$$\swarrow\,\,(dz\,\,direction)$$
$$:\,-\hat{y}\int_\,d\,xd\,z\,\,\times\,\,[\int_\,(V_x-\frac{\partial V_{x}}{\partial y}\,\frac{dy}{2})\hat{y}\,+\,\int_\,(V_z\,+\frac{\partial V_{z}}{\partial y}\,\frac{dy}{2}\hat{z})] $$
$$=\,-\int_\,(V_x-\frac{\partial V_{x}}{\partial y}\,\frac{dy}{2})\,dxdz\,\hat{z}\,+\,\int_\,(V_z\,+\,\frac{\partial V_z}{\partial y}\,\frac{dy}{2})\,dxdz\,\hat{x} $$
$$\nearrow\,\,(dz\,\,direction)$$
$$=\,\int_\,(V_x+\frac{\partial V_{x}}{\partial y}\,\frac{dy}{2})\,dxdz\,\hat{z}\,-\,\int_\,(V_z\,-\,\frac{\partial V_z}{\partial y}\,\frac{dy}{2})\,dxdz\,\hat{x} $$
$$\therefore,\,\swarrow+\,\nearrow\,=\,\frac{\partial V_{z}}{\partial y}\,dxdydz\hat{x}-\,\frac{\partial V_{x}}{\partial y}\,dxdydz\hat{z} $$
(3)
$$\Downarrow\,\,(dy\,\,direction)$$
$$:\,-\hat{z}\int_\,d\,xd\,y\,\,\times\,\,[\int_\,(V_x-\frac{\partial V_{x}}{\partial z}\,\frac{dz}{2})\hat{x}\,+\,\int_\,(V_y\,+\frac{\partial V_{y}}{\partial z}\,\frac{dz}{2}\hat{y})] $$
$$=\,-\int_\,(V_x-\frac{\partial V_{x}}{\partial z}\,\frac{dz}{2})\,dxdy\,\hat{y}\,+\,\int_\,(V_y\,+\,\frac{\partial V_y}{\partial z}\,\frac{dz}{2})\,dxdy\,\hat{x} $$
$$\Uparrow\,\,(dy\,\,direction)$$
$$=\,\int_\,(V_x+\frac{\partial V_{x}}{\partial z}\,\frac{dz}{2})\,dxdy\,\hat{y}\,-\,\int_\,(V_y\,-\,\frac{\partial V_y}{\partial z}\,\frac{dz}{2})\,dxdy\,\hat{x} $$
$$\therefore,\,\Downarrow+\,\Uparrow\,=\,\frac{\partial V_{x}}{\partial z}\,dxdydz\hat{y}-\,\frac{\partial V_{y}}{\partial z}\,dxdydz\hat{x} $$
dx, dy, dz 방향의 양을 전부 더하면 (1) + (2) + (3)이 된다. 이 때 적분기호를 예와 같이 빼주면 이는
$$[(\frac{\partial V_z}{\partial y}-\frac{\partial V_y}{\partial z})\hat{x}\,+\,(\frac{\partial V_x}{\partial z}-\frac{\partial V_z}{\partial x})\hat{y}\,+\,(\frac{\partial V_y}{\partial x}-\frac{\partial V_x}{\partial y})\hat{z}]dxdydz $$
그러면 Curl(V)는 아래와 같다는 것이 증명되었다.
$$\nabla\times\,\mathbb{V}\,\,=\,\,\lim_{\int_\,d\tau \to 0}\frac{\int_\,d\sigma\,\times\,\mathbb{V}}{\int_\,d\tau} $$

4. Laplacian

<div class="separator" style="clear: both; text-align: center;"><a href="https://3.bp.blogspot.com/-wTEihctENx4/WkshkCwlfNI/AAAAAAAAScg/CogdBjEHbswPXYSfpLAHlhOjLI4x9EUKQCLcBGAs/s1600/Continuity%2BEquation%2B-%2BControl%2BVolume.jpg" imageanchor="1" style="margin-left: 1em; margin-right: 1em;"><img border="0" src="https://3.bp.blogspot.com/-wTEihctENx4/WkshkCwlfNI/AAAAAAAAScg/CogdBjEHbswPXYSfpLAHlhOjLI4x9EUKQCLcBGAs/s640/Continuity%2BEquation%2B-%2BControl%2BVolume.jpg" width="640" height="359" data-original-width="590" data-original-height="331" /></a></div>
어떤 함수 Φ를 정의할 때, Φ의 Laplacian ∇^2_Φ는 다음과 같다.
$$\nabla^2 \phi\,=\lim_{\int_\,d\tau \to 0}\frac{\int_\,\nabla\phi\,d\sigma}{\int_\,d\tau} $$

(1)$$\Leftarrow\,\,(dx\,\,direction)\,:\,\nabla\phi_x\,=\,$$
$$(\frac{\partial \phi}{\partial x}-\frac{dx}{2}\frac{\partial^2 \phi}{\partial x^2})\hat{x}+(\frac{\partial \phi}{\partial y}-\frac{dy}{2}\frac{\partial^2 \phi}{\partial y^2})\hat{y}+(\frac{\partial \phi}{\partial z}-\frac{dz}{2}\frac{\partial^2 \phi}{\partial z^2})\hat{z},$$
$$d\sigma_x\,=\,-dydz\hat{x} $$
$$\Rightarrow\,\,(dx\,\,direction)\,:\,\nabla\phi_x\,=\,$$
$$(\frac{\partial \phi}{\partial x}+\frac{dx}{2}\frac{\partial^2 \phi}{\partial x^2})\hat{x}+(\frac{\partial \phi}{\partial y}+\frac{dy}{2}\frac{\partial^2 \phi}{\partial y^2})\hat{y}+(\frac{\partial \phi}{\partial z}+\frac{dz}{2}\frac{\partial^2 \phi}{\partial z^2})\hat{z},$$
$$d\sigma_x\,=\,dydz\hat{x} $$
$$\therefore,\,\Leftarrow+\Rightarrow\,=\,\frac{\partial^2 \phi}{\partial x^2}dxdydz $$
(2)
$$\swarrow\,\,(dz\,\,direction)\,:\,\nabla\phi_z\,=\,$$

$$(\frac{\partial \phi}{\partial x}-\frac{dx}{2}\frac{\partial^2 \phi}{\partial x^2})\hat{x}+(\frac{\partial \phi}{\partial y}-\frac{dy}{2}\frac{\partial^2 \phi}{\partial y^2})\hat{y}+(\frac{\partial \phi}{\partial z}-\frac{dz}{2}\frac{\partial^2 \phi}{\partial z^2})\hat{z},$$
$$d\sigma_z\,=\,-dxdz\hat{y} $$
$$\nearrow\,\,(dz\,\,direction)\,:\,\nabla\phi_z\,=\,$$

$$(\frac{\partial \phi}{\partial x}+\frac{dx}{2}\frac{\partial^2 \phi}{\partial x^2})\hat{x}+(\frac{\partial \phi}{\partial y}+\frac{dy}{2}\frac{\partial^2 \phi}{\partial y^2})\hat{y}+(\frac{\partial \phi}{\partial z}+\frac{dz}{2}\frac{\partial^2 \phi}{\partial z^2})\hat{z},$$

$$d\sigma_z\,=\,dxdz\hat{y} $$
$$\therefore,\,\swarrow+\nearrow\,=\,\frac{\partial^2 \phi}{\partial y^2}dxdydz $$
(3)
$$\Downarrow\,\,(dy\,\,direction)\,:\,\nabla\phi_y\,=\,$$
$$(\frac{\partial \phi}{\partial x}-\frac{dx}{2}\frac{\partial^2 \phi}{\partial x^2})\hat{x}+(\frac{\partial \phi}{\partial y}-\frac{dy}{2}\frac{\partial^2 \phi}{\partial y^2})\hat{y}+(\frac{\partial \phi}{\partial z}-\frac{dz}{2}\frac{\partial^2 \phi}{\partial z^2})\hat{z},$$
$$d\sigma_y\,=\,-dxdy\hat{z} $$
$$\Uparrow\,\,(dy\,\,direction)\,:\,\nabla\phi_y\,=\,$$</p>

$$(\frac{\partial \phi}{\partial x}+\frac{dx}{2}\frac{\partial^2 \phi}{\partial x^2})\hat{x}+(\frac{\partial \phi}{\partial y}+\frac{dy}{2}\frac{\partial^2 \phi}{\partial y^2})\hat{y}+(\frac{\partial \phi}{\partial z}+\frac{dz}{2}\frac{\partial^2 \phi}{\partial z^2})\hat{z},$$
$$d\sigma_y\,=\,dxdy\hat{z} $$
$$\therefore,\,\swarrow+\nearrow\,=\,\frac{\partial^2 \phi}{\partial z^2}dxdydz $$
(1),(2),(3)을 모두 더하면 다음과 같다.
$$\nabla\,\phi\,d\sigma\,=\,(\frac{\partial^2 \phi}{\partial x^2}\,+\,\frac{\partial^2 \phi}{\partial y^2}\,+\frac{\partial^2 \phi}{\partial z^2})dxdydz $$
적분기호를 제거하고 d(tau)로 나누어주면 아래와 같이 증명이 완료된다.
$$\nabla^2 \phi\,=\lim_{\int_\,d\tau \to 0}\frac{\int_\,\nabla\phi\,d\sigma}{\int_\,d\tau} $$
이로서 Cartesian Coordinates에서 Grad, Curl, Div, Laplacian에 대한 표현형을 소개했고 그것이 성립한다는 데에 대한 증명을 끝냈다.



* 참고 자료
1. Mathematical Methods for Physicists, 1st ed., ARFKEN & WEBER, ch.1, Vector analysis, p. 58<
2. In the same book, p. 63





