---
layout: post
title: test math2
categories: dl
description: Feugiat amet tempus
image: assets/images/pic06.jpg
---

## Integrals

#### 2D Integrals

projezierbarkeit x, y

#### 3D Integrals

$G\subseteq \Bbb{R^3}$

projezierbarkeit x, y

###### Volume

$$
V = \iiint\limits_G 1\,d(x, y, z)
$$

###### Mass

$$
M := \iiint\limits_G ρ(x, y, z)d(x, y, z)
$$

###### Schwerpunkt

$$
x_s = \frac{1}{M}\iiint\limits_G xρ(x, y, z)d(x, y, z) \\
y_s = \frac{1}{M}\iiint\limits_G yρ(x, y, z)d(x, y, z) \\
z_s = \frac{1}{M}\iiint\limits_G zρ(x, y, z)d(x, y, z)
$$



###### Trägheuitsmomente

$$
T_x = \frac{1}{M}\iiint\limits_G (y 2 + z 2 )ρ(x, y, z)d(x, y, z) \\
T_y = \frac{1}{M}\iiint\limits_G (x 2 + z 2 )ρ(x, y, z)d(x, y, z) \\
T_z = \frac{1}{M}\iiint\limits_G (x 2 + y 2 )ρ(x, y, z)d(x, y, z)
$$
#### Coordinate transformations

|            polar/ cylindric            |                            sphere                            |
| :------------------------------------: | :----------------------------------------------------------: |
| $$x=rcos\varphi\\ y=rsin\varphi\\z=t$$ | $$x=rsin\vartheta cos\varphi\\ y=rsin\vartheta sin\varphi\\ z=rcos\vartheta$$ |
|             $$ |det| = r$$             |                $$|det| =r^{2}sin\vartheta $$                 |

#### Determinant

$$
|A| = \begin{vmatrix}a & b\\c & d\end{vmatrix} = ad - bc
$$



*Example:*
$$
H = \{(r,\varphi)\in\Bbb{R}²|1\leq{r}\leq 2,0\leq \varphi \leq \pi\}
$$

$$
det\biggl(\frac{\partial(x,y)}{\partial(r,\varphi)}\biggr) = \biggl(\begin{matrix}cos\varphi & -rsin\varphi\\sin\varphi & rcos\varphi\end{matrix}\biggr) =rcos²\varphi+rsin²\varphi=r
$$



#### Curve Integrals

Parametrization
$$
k(t)=\biggl(\begin{matrix}k_1(t) \\ k_2(t)\end{matrix}\biggr), \,\,\, \in[a,b]
$$
Arclength
$$
L=\int\limits_K 1 \, dk=\int\limits_a^b ||\dot{\vec{k}}||\, dt
$$
Skalarfield (non orientated curves)
$$
\int\limits_K f \, dk=\int\limits_a^b f(\vec{k}(t))\,||\dot{\vec{k}}||\, dt
$$



#### Surface Interals

$$
\vec{n} = \pm \frac{\vec{x_u} \times \vec{x_v}}{||\vec{x_u} \times \vec{x_v}||}
$$



#### Gauß

regulärer Bereich, Oberfläche S, Parameterdarstellung so gewählt (+-n) dass normale nach außen zeigt, stetig differenzierbar, abl 1 o



​						Volumen $\lrarr ​$ Oberfläche

​			Quelldichte im Körper $\lrarr $ Fluss des Vektorfeldes durch Oberfläche
$$
￼
\int\limits_G div(\vec V ) \, dV=\int\limits_S (\vec{V} \circ \vec{n})\, dS
$$

$$
div \,\vec V = \frac{\partial V_1}{\partial x}+\frac{\partial V_2}{\partial y}+\frac{\partial V_3}{\partial z}
$$



#### Stokes / Green

gilt für stückweise glatte, zweiseitige fläche mit geschlossener randkurve ohne doppelpunkte mit auf mengo o stetig partielle abl 1 ord

Dabei ist dierandkurve im uhrzeiger sinn fest gelegt--- fläche S muss beim durchlaufen links liegen.

​						Fläche $\lrarr $ Kurve (Rand)
$$
\int\limits_S rot(\vec{V}) \circ \vec{n} \, dS = \oint\limits_{\partial{S}} \vec V  \, \vec{dK}
$$

$$
rot(\vec V ) = \begin{pmatrix}\frac{\partial V_3}{\partial y}-\frac{\partial V_2}{\partial z}\\ \frac{\partial V_1}{\partial z}-\frac{\partial V_3}{\partial x}\\ \frac{\partial V_2}{\partial x}-\frac{\partial V_1}{\partial y} \end{pmatrix}
$$



#### Complex Integrals

###### Functions in $$ \Bbb{C} $$

$$ z=x+jy ​$$

$f(z)=f(x+jy)=\Re\{f(z)\}+\Im\{f(z)\} = u(x,y) + jv(x,y)$

$z=rcos\varphi+jrsin\varphi = re^{j\varphi}$

*examples:*

$z* \overline z = (x+jy)(x-jy) = x^2+y^2​$

$(z²+1)=(z-i)(z+i)$

$(z²-1) = (z-1)(z+1)$

###### Limits and differentiation in $\Bbb{C}$

A complex function f is ***holomorphic***, regular or analytical if,

1) a point $z_0 \in D(f)​$ exists on an open set $\mathcal{O}​$ so that $z_0 \in \mathcal{O}\subseteq D(f)​$ is valid and $f​$ is differentiable in every point of $\mathcal{O}​$.

2)  ...

3) it is expressed as a polynomial of the form $f(z) = z^n​$ or a power series of the form $f(z)=\sum_{n=0}^{\infty}c_n z^n​$
$$
f^{'}=\lim_{z\to z_0} \frac{f(z)-f(z_0)}{z-z_0}
$$


###### Cauchy-Riemann Differential Equations

Notwendiges aber kein hinreichendes Kriterium für die komplexe Integration.
$$
u_x (x_0 , y_0) = v_y ( x_0 , y_0)\\
u_y (x_0 , y_0) = - v_x ( x_0 , y_0)\\
f^{'}(z_0)=u_x (x_0 , y_0)+ jv_x ( x_0 , y_0)=u_y (x_0 , y_0)-jv_y ( x_0 , y_0)
$$

*example*:
$$
f(z)=z\overline z=x^2+y^2 = u(x,y) \\
v_x(x,y) = v_y(x,y) = 0 \\
u_x(x,y) = 2x, and \,\,u_y(x,y)=2y \\
\implies z_0=0 \,\,with\,\,x_0=y_0=0 \,\, differentiable
$$
*just differentiable at postition zero*

###### Residuals

Singularities sind die komplexen Nullstellen des Nenners bei gebrochen rationalen Funktionen e.g. $\frac{1}{(z-j)(z+j)}​$ with $z_0 = j; z_1=-j​$ as singularities.
$$
f(z)= \lim_{z\to z_0}(z-z_0)f(z)
$$


###### Resiudal sentence

Residuensatz mit Bedingungen stückweise glatte geschlossene doppelpunktfreie Kurve, sodass alle Singularitäten im inneren liegen. Der Drehsinn ist hierbei so zu wählen das das Innere links der Kurve liegt.
$$
\ointctrclockwise\limits_K{f(z)}\,dz = 2\pi j \sum_{i=1}^{n}Res_{z=z_i} f(z)
$$

*example*:
