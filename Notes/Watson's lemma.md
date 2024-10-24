Consider: $F(x)=\int_{0}^Tf(t)e^{-xt}dt$
Suppose $f(t)\sim t^\alpha \sum_{n=0}^{\infty}a_{n}t^{n\beta}$ as $t\to 0^{+}$ with $\alpha>-1$ and $\beta>0$
Suppose also either: 
- $\lvert f(t) \rvert<Ke^{bt}$ for all $t>0$ and some $K,b>0$
OR
- $\int _0^T\lvert f(t) \rvert dt<\infty$
Then 
$$
F(x)\sim \sum_{n=0}^{\infty} a_{n} \frac{\Gamma(\alpha+\beta n+1)}{x^{\alpha+\beta n+1}}
$$

#### Proof
No elegance, just suffering
$$
\begin{align}
F(x) & =\int_{0}^\epsilon fe^{-xt}dt+\int_{\epsilon}^Tfe^{-xt}dt \\
 & =F_{1}+F_{2}
\end{align}
$$
##### Step 1
Show $F_{2}$ is small
###### Case 1
