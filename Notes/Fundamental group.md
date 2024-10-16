### Proposition
Given [[Paths|paths]]:
$$
\begin{align}
\gamma_{0}:x_{0}\leadsto x_{1} \\
\gamma_{1}:x_{1}\leadsto x_{2} \\
\gamma_{2}:x_{2}\leadsto x_{3}
\end{align}
$$
The following hold:
1. $(\gamma_{0}\cdot \gamma_{1})\cdot \gamma_{2}\simeq \gamma_{0}\cdot(\gamma_{1}\cdot \gamma_{2})$ relative to $\{ 0,1 \}$
2. $\gamma_{0}\cdot c_{x_{0}}\simeq \gamma_{0}$ relative to $\{ 0,1 \}$
3. $\gamma_{0}\cdot \gamma_{0}^{-1}\simeq c_{x_{0}}$ relative to $\{ 0,1 \}$
#### Proof
(1) Let $t$ interpolate between paths and $s$ be the path variable.
Consider the following image:
```
^
|---0---|-1-|-2-|
|
t
|
|-0-|-1-|---2---|
*------s-------->
```
If we linearly scaled the bottom intervals to the top ones, the interval lengths would be (as a function of $t$): $t+1\over 4$, $\frac{1}{4}$, $2-t\over 4$.
This motivates the homotopy:
$$
H(s,t)=\begin{cases}
\gamma_{0}\left( \frac{4s}{t+1} \right) & s\leq \frac{t+1}{4} \\
\gamma_{1}\left(4s - t-1\right) & {t+1\over 4}\leq s\leq {t+2\over 4} \\
\gamma_{2}({4s\over 2-t} - {t+2\over 2-t}) & {t+2\over 4}\leq s
\end{cases}
$$
(2) Same strategy, with the following image
```
---0---
-0-|-c-
```
Interval lengths: $t+1\over 2$ and $1-t\over 2$
$$
H(s,t)=\begin{cases}
\gamma_{0}\left( \frac{2s}{t+1} \right) & s\leq {t+1\over 2} \\
x_{1} & s\geq {t+1\over 2}
\end{cases}
$$
(3) Now this one is a bit different, but also easier. We will just make paths that go up to $\gamma_{0}(1-t)$ and back.
$$
H(s,t)=\begin{cases}
\gamma_{0}(2s) & s\leq{1-t\over 2} \\
\gamma_{0}(1-t)  & {1-t\over 2} \leq s\leq {1+t\over 2} \\
\gamma_{0}(2-2s) & {1+t\over 2} \leq s
\end{cases}
$$

### Theorem
Let $X$ be a space and $x_{0}$ a point. Let $\pi_{1}(X,x_{0})$ be the set of homotopy classes of loops in $X$ based at $x_{0}$. Then using
$$
[\gamma]\cdot[\gamma']=[\gamma \cdot \gamma']
$$
gives a group structure
#### Proof
Directly from previous proposition.

### Definition
$\pi_{1}(X,x_{0})$ is the fundamental group of $X$ based at $x_{0}$.
### Definition
- Based space is a pair $(X,x_{0})$ where $X$ is a space, and $x_{0}\in X$ is the basepoint.
- Map of based spaces $f:(X,x_{0})\to(Y,y_{0})$ is a map $f:X\to Y$ st $f(x_{0})=y_{0}$.
- Based homotopy is a homotopy relative to $\{ x_{0} \}$.
### Proposition
Let $f:(X,x_{0})\to (Y,y_{0})$ be a based map. Then the function
$$
\begin{align}
\pi_{1}(f):\pi_{1}(X,x_{0})&\to \pi_{1}(Y,y_{0}) \\
[Y]&\to [f\circ Y]
\end{align}
$$
is well defined and satisfies:
1. $\pi_{1}(f)$ is a group homomorphism
2. $f$ based homotopic to $f'$ $\implies \pi_{1}(f)=\pi_{1}(f')$
3. If $(A,a)\to_{h}(B,b)\to_{k}(C,c)$ based maps, then $\pi_{1}(k\circ h)=\pi_{1}(k)\circ \pi_{1}(h)$
4. $\pi_{1}(id_{X})=id_{\pi_{1}(X)}$
#### Proof
Well defined? If $\gamma \simeq \gamma'$ as paths, then $f\circ \gamma \simeq f\circ \gamma'$ as paths.
1. $f\circ c_{x_{0}}=c_{y_{0}}\implies \pi_{1}(f)$ preserves unit
   $f\circ(\gamma \cdot \gamma')=(f\circ \gamma)\cdot(f\circ \gamma')\implies$ composition law respected
2. $f\simeq f'$ relative to $\{ x_{0} \} \implies f\circ \gamma \simeq f'\circ \gamma$ relative to $\{ 0,1 \}$
3. $\pi_{1}(k\circ h)[\gamma]=[k\circ h\circ \gamma]=\pi_{1}(k)[h\circ \gamma]=\pi_{1}(k)\circ \pi_{1}(h)[\gamma]$ for all $\gamma \in \pi_{1}(A,a)$
4. $\pi_{1}(id_{X})[\gamma]=[id_{x}\gamma]=[\gamma]$ for all $\gamma \in \pi_{1}(X,x_{0})$
### Notation
$f_{*}=\pi_{1}(f)$
### Proposition
$u:x_{0}\leadsto x_{1}$ path in $X$ induces a group isomorphism
$$
\begin{align}
u_{\#}:\pi_{1}(X,x_{0})&\to \pi_{1}(X,x_{1}) \\
[\gamma]&\to [u^{-1}\cdot \gamma \cdot u]
\end{align}
$$
(intuitively, we just go from $x_{1}$ to $x_{0}$, then do the loop $\gamma$ and then go back to $x_{1}$ along the same path)
It satisfies:
1. $u\simeq u'$ as paths $\implies u_{\#}=u_{\#}'$
2. $(c_{x_{0}})_{\#}=id_{\pi_{1}(X,x_{0})}$
3. If $v:x_{1}\leadsto x_{2}$, then $(u\cdot v)_{\#}=v_{\#}\circ u_{\#}$
4. If $f:X\to Y$ st $f(x_{0})=y_{0}$ and $f(x_{1})=y_{1}$ then the following diagram commutes:
```tikz
\usepackage{tikz-cd}

\begin{document}
\begin{tikzcd}
\pi_1(X,x_0) \arrow[r,"f_*"] \arrow[d,"u_{\#}"] & \pi_1(Y,y_0)\arrow[d,"(f\circ u)_{\#}"]\\
\pi_1(X,x_1)\arrow[r, "f_*"] & \pi_1(Y,y_1)
\end{tikzcd}
\end{document}
```
5. If $x_{1}=x_{0}$, $u_{\#}$ is automorphism of $\pi_{1}(X,x_{0})$ given by conjugation in $[u]\in \pi_{1}(X,x_{0})$
#### Proof
$$
\begin{align}
(f\circ u)_{\#}\circ f_{*} [\gamma]&=(f\circ u)_{\#}[f\circ \gamma] \\
&=[(f\circ u)^{-1}\cdot(f\circ \gamma)\cdot(f\circ u)] \\
&=[(f\circ u^{-1})\cdot(f\circ \gamma)\cdot(f\circ u)] \\
&=[f\circ(u^{-1}\cdot \gamma \cdot u)] \\
 & =[f\circ u_{\#}(\gamma)] \\
 & =f_{*}([u_{\#}(\gamma)])
\end{align}
$$
### Warning
$X$ path connected $\implies \pi_{1}(X,x_{0})\cong\pi_{1}(X,x_{1})$ NOT a cannonical isomorphism, it depends on path $x_{0}\leadsto x_{1}$.
NB Abstract properties eg being trivial, abelian, ... make sense without specifiying $x_{0}$

### Lemma
$f,g:X\to Y$, $f\simeq_{H}g$, $x_{0}\in X$. Then define $u=H(x_{0},\cdot):f(x_{0})\leadsto g(x_{0})$. 
Then the following diagram commutes:
```tikz
\usepackage{tikz-cd}
\begin{document}
\begin{tikzcd}
\pi_1(X,x_0) \arrow[r,"f_*"] \arrow[rd, "g_*"] & \pi_1(Y,f(x_0)) \arrow[d, "u_{\#}"]\\
& \pi_1(Y,g(x_0))
\end{tikzcd}
\end{document}
```

#### Proof
##### Idea
For a path $\gamma$ in $X$ based at $x_{0}$ we want to construct the following two paths in $Y$ based at $g(x_{0})$ and prove that they are homotopy equivalent.
```
gx0---gogamma---->gx0
|                  ^
|                  |
u^-1               u
|                  |
|                  |
V                  |
fx0----fogamma--->fx0
```
Note that $f\circ \gamma=H(\cdot,0)\circ \gamma$ and $g\circ \gamma=H(\cdot,1)\circ \gamma$
We literally put coordinates $I\times I$ on this square.

##### Step 1
$l^+:I\to I\times I$ with $s\to(s,1)$
$l^-:I\to I\times I$ by concatenating:
$s\to(0,1-s)$, $s\to(s,0)$ and $s\to(1,s)$
Then $l^+\simeq_{L} l^-$ relative to $\{ 0,1 \}$ where $L(s,\lambda)=\lambda l^-(s)+(1-\lambda)l^+(s)$

##### Step 2
Let $\gamma$ be a loop based at $x_{0}$ in $X$. 
Set $G: I\times I\to_{\gamma \times id}X\times I\to_{H}Y$.
So $G(t,0)=f\circ \gamma$ and $G(t,1)=g\circ \gamma$ and 
$G(0,t)=H(x_{0},t)=u(t)$
$G\circ l^+\simeq G\circ l^-$ relative to $\{ 0,1 \}$ ie as paths from $g(x_{0})$ to $g(x_{0})$
$[G\circ l^+]=[g\circ \gamma]$ and $[G\circ l^-]=[u^{-1}\cdot(f\circ \gamma)\cdot u]$ so done.

### Theorem
$f:X\to Y$ homotopy equivalence, $x_{0}\in X$
Then $f_{*}:\pi_{1}(X,x_{0})\to \pi_{1}(Y,f(x_{0}))$ is an isomorphism
#### Proof
Let $g:Y\to X$ homotopy inverse of $f$. Say $id_{X}\simeq_{H} g\circ f$.
Let $u(t)=H(x_{0},t)$, a path in $X$ from $x_{0}$ to $g(f(x_{0}))$. 
By previous lemma $(g\circ f)_{*}=u_{\#}\circ(id_{X})_{*}$ 
(where functions are from $X$ to $X$)
Also $u_{\#}$ is an isomorphism so 
$\pi_{1}(X,x_{0})\to _{f_{*}}\pi_{1}(Y,f(x_{0}))\to_{g_{*}}\pi_{1}(X,g\circ f(x_{0}))$
So the first map is injective, while the second is surjectvie because there is an isomorphism $u_{\#}$. 
$u_{\#}:\pi_{1}(X,x_{0})\to \pi_{1}(X,g\circ f(x_{0}))$
Reverse roles of $f$ and $g$:
$f_{*}:\pi_{1}(X,g\circ f(x_{0}))\to \pi_{1}(X,f\circ g\circ f(x_{0}))$ surjective
Commutative diagram remarkable 

### Definition
$X$ is simply connected if it is path connected and its fundamental group is trivial in some (hence all) basepoints.

### Lemma
$X$ simply connected $\iff$ For each pair of points $x_{0},x_{1}\in X$ there is a uninque homotopy class of paths between them.
#### Proof
$(\implies)$ Suppose $X$ is simply connected. Let $x_{0},x_{1}\in X$. $X$ is path connected so have path $x_{0}\leadsto x_{1}$. Suppose $\gamma,\gamma':x_{0}\leadsto x_{1}$. Then $\gamma ^{-1}\cdot \gamma$ is a loop based at $x_{0}$. 
$[\gamma ^{-1}\cdot \gamma]\in \pi_{1}(X,x_{0})=\{ [c_{x_{0}}] \}$. So $\gamma ^{-1}\cdot \gamma'\simeq c_{x_{0}}$ relative to the endpoints
$\implies \gamma'\simeq \gamma \cdot c_{x_{0}}\simeq \gamma$ as loops based at $x_{0}$
$(\impliedby)$ Existence of paths between any 2 points implies $X$ is path connected. Suppose $\gamma$ is a loop based at $x_{0}$. The loop is homotopic to the constant loop at $x_{0}$ so $\pi_{1}(X,x_{0})=\{ * \}$.