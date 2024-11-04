Laplace integrals are of the form:
$$
I(x)=\int_{a}^b f(t)e^{x\phi(t)}dt
$$
where $f$ and $\phi$ are nice enough

Note that [[Watson's lemma]] deals with the special case $\phi=-t$ (and $a=0$, $b=T$, so the endpoint dominates the integral)

## Principle of localisation
The [[Asymptotic Expansion]] of $I$ as $x\to \infty$ is determined by contributions from very small regions around the maximum of $\phi$.

### Case monotonic
Suppose $\phi$ is monotonic on $[a,b]$
Let $\phi'(t)>0$ and let $f(b)\neq 0$.
Then the integral is dominated by a nbd of $b$:
Let $u=\phi(t)$ and $t=\phi ^{-1}(u)$
$$
\implies I=\int_{\phi(a)}^{\phi(b)} \frac{f(t)}{\phi'(t)} e^{xu} du
$$
Can use [[Watson's lemma]] or just use partial integration:
$$
I(x)\sim \frac{f(b)e^{x\phi(b)}}{x\phi'(b)}
$$
If $\phi'(t)<0$ and $f(a)\neq 0$ 
$$
\implies I(x)\sim  \frac{f(a)e^{x\phi(a)}}{x\lvert \phi'(a) \rvert }
$$
### Case one max
Suppose $\phi$ has one internal maximum at $t=c$ (and this is the absolute maximum) st $\phi'(c)=0$ and $\phi''(c)<0$ and $f(c)\neq 0$.
$$
\begin{gather}
I(x)=\int_{c-\epsilon}^{c+\epsilon}f(t)e^{x\phi(t)}dt+\int_{\Omega_{\epsilon}}f(t)e^{x\phi}dt\\
=I_{1}+I_{2}
\end{gather}
$$
$$
I_{2}=\int_{c+\epsilon}^b f(t)e^{ x\phi(t) }dt+\int_{a}^{c-\epsilon}f(t)e^{ x\phi(t) }dt=O\left( \frac{1}{x}e^{ x\phi(c+\epsilon) } \right)+O\left( \frac{1}{x}e^{ x\phi(c-\epsilon) } \right)
$$
From the [[#Case monotonic]].

Then $I_{2}\ll \frac{e^{ x }\phi(c)}{x}$ by noting that $\phi(c+\epsilon)<$