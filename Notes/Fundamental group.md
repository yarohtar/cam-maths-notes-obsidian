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
Let $f:(X,x_{0})\to (Y,y_{0})$ be a based map. Then the fct (?) 
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
2. $f\simeq f'$ rerlative to $\{ x_{0} \} \implies f\circ \gamma \simeq f'\circ \gamma$ relative to $\{ 0,1 \}$
3. $\pi_{1}(k\circ h)[\gamma]=[k\circ h\circ \gamma]=\pi_{1}(k)[h\circ \gamma]=\pi_{1}(k)\circ \pi_{1}(h)[\gamma]$ for all $\gamma \in \pi_{1}(A,a)$
4. $\pi_{1}(id_{X})[\gamma]=[id_{x}\gamma]=[\gamma]$ for all $\gamma \in \pi_{1}(X,x_{0})$
### Notation
$f_{*}=\pi_{1}(f)$
### Proposition
$ux_{0}\leadsto x_{1}$ path in $X$ induces a group isomorphism
$$
\begin{align}
u_{\#}:\pi_{1}(X,x_{0})&\to \pi_{1}(X,x_{1}) \\
[\gamma]&\to [u^{-1}\cdot \gamma \cdot u]
\end{align}
$$
such that
1. $u\simeq u'$ as paths $\implies u_{\#}=u_{\#}'$
2. $(c_{x_{0}})_{\#}=id_{\pi_{1}(X,x_{0})}$
3. If $v:x_{1}\leadsto x_{2}$, then $(u\cdot v)_{\#}=v_{\#}\circ u_{\#}$
4. If $f:X\to Y$ st $f(x_{0})=y_{0}$ and $f(x_{1})=y_{1}$ then
(commutes, remarkable)
5. If $x_{1}=x_{0}$, $u_{\#}$ is automorphism of $\pi_{1}$