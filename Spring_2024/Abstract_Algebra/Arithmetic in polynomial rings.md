---
tags:
  - abstract-algebra
---

# 4.1 Polynomial Arithmetic and the Division Algorithm

Let $R$ be a ring $A$ **polynomial with coefficients in $R$** is an expression of the form
$$a_0+a_1x+a_2x^2+\cdots+a_nx^n$$
for each $a_i\in R$, $a_n\ne0_R$, and $x$ an "*unknown*". 
*$x$ can be anything, a matrix, integer, rational, object*.

We call $R[x]=\{\text{polynomials\;with\;coefficients\;in\;R}\}$.

## Example

Compare $R[x]$ to

- $\mathbb{Z}[\sqrt{2}]=\{a+b\sqrt{2}|a,b,\in\mathbb{Z}\}$
- $\mathbb{R}[i]=\{a+bi|a,b\in\mathbb{R}\}\cong\mathbb{C}$

Arithmetic in $R[x]$ is performed in the familiar way … Theorem 4.1 assures us everything is well-defined!

## Example

$(a)$ Evaluate $(x+1)^2$ in $\mathbb{Z}[x]$.

$(b)$ Evaluate $(x+1)^2$ in $\mathbb{Z}_2[x]$.

$(a)$ In $\mathbb{Z}[x]$,

$$\begin{align*}
(x+1)^2=(x+1)(x+1)\\
=(x+1)\cdot x+(x+1)\cdot 1\\
=x^2+x+x\cdot 1+1\cdot 1\\
=x^2+2x+1.
\end{align*}$$

$(b)$ In $\mathbb{Z}_2[x]$,

$$\begin{align*}
(x+1)^2=(x+1)\cdot(x+1)\\
=x^2+x\cdot 1+1\cdot x+1\cdot 1\\
=1x^2+2x+1\\
=x^2+0x+1\\
=x^2+1.
\end{align*}$$


## Theorem 4.6 (Polynomial division)

Let $F$ be a field and $f(x),g(x)\in F[x]$ with $g(x)\ne0_F.$ Then,
$\exists!q(x),r(x)\in F[x]$ such that
- $f(x)=g(x)\cdot q(x)+r(x)$ and
-  $deg[r(x)]<deg[g(x)]$ or $r(x)=0_F$.
