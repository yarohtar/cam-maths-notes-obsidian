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
Now find:
$$
\begin{align}
H(s,0)&=\begin{cases}
\gamma_{0}(4s) & 0\leq s\leq \frac{1}{4} \\
\gamma_{1}\left( 4s+\frac{1}{4} \right) & \frac{1}{4}\leq s\leq \frac{1}{2} \\
\gamma_{2}\left( 2s+\frac{1}{2} \right)  & \frac{1}{2}\leq s\leq 1
\end{cases} \\
H(s,1)&=\begin{cases}
\gamma_{0}(2s) & 0\leq s\leq \frac{1}{2} \\
\gamma_{1}\left( 4s+\frac{1}{2} \right) & \frac{1}{2}\leq s\leq \frac{3}{4} \\
\gamma_{2}\left( 4s+\frac{3}{4} \right) & \frac{3}{4}\leq s
\end{cases}
\end{align}
$$

### Theorem
Let $X$ be a space and $x_{0}$ a point. Let $\pi_{1}(X,x_{0})$ be the set of homotopy classes of loops in $X$ based at $x_{0}$. Then using
$$
[\gamma]\cdot[\gamma']=[\gamma \cdot \gamma']
$$
gives a group structure
#### Proof
Directly from previous proposition.