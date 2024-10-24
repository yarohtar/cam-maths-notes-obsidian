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
$\lvert F_{2} \rvert\leq \int_{\epsilon}^TKe^{bt-xt}\leq \int_{\epsilon}^\infty Ke^{bt-xt}$
Assuming $x>b$ we can integrate this and get
$\lvert F_{2} \rvert\leq \frac{K}{x-b}e^{(b-x)\epsilon}$ ie $\lvert F_{2} \rvert=O\left( \frac{e^{-\epsilon x}}{x} \right)$#
###### Case 2
$\lvert F_{2} \rvert\leq \int_{\epsilon}^T\lvert f \rvert e^{-xt}dt\leq e^{-\epsilon x}\int_{\epsilon}^T\lvert f \rvert dt$
So $\lvert F_{2} \rvert=O(e^{-\epsilon x})$

In both cases, $F_{2}$ is small beyond all orders.

##### Step 2
Want to show
$$
\frac{F_{1}-\sum a_{n} \frac{\Gamma(\alpha+\beta n+1)}{x^{\alpha+\beta n+1}}}{x^{-\alpha-\beta n-1}}\to 0
$$
Using a property of [[The Gamma Function]] we find that the numerator is equal to:
$$
\left\lvert  \int_{0}^tfe^{-xt}dt-\int_{0}^\infty \sum^Na_{n}t^{\alpha+\beta n}e^{-}  \right\rvert 
$$