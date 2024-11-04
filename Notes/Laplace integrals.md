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
\begin{align}

I_{2} & =\int_{c+\epsilon}^b f(t)e^{ x\phi(t) }dt+\int_{a}^{c-\epsilon}f(t)e^{ x\phi(t) }dt \\
 & =O\left( \frac{1}{x}e^{ x\phi(c+\epsilon) } \right)+O\left( \frac{1}{x}e^{ x\phi(c-\epsilon) } \right)
\end{align}
$$
From the [[#Case monotonic]].

Then $I_{2}\ll \frac{e^{ x }\phi(c)}{x}$ by noting that $\phi(c+\epsilon)<\phi(c)$ and $\phi(c-\epsilon)<\phi(c)$

Now Taylor expand $f$ and $\phi$.
$$
\phi(t)=\phi(c) + \frac{1}{2}\phi''(c)(t-c)^{2}+\dots
$$
$$
f(t)=f(c)+O(t-c)
$$

$$
\begin{align}
I_{1} & =\int_{c-\epsilon}^{c+\epsilon}[f(c)+\dots]\exp\left( x\phi(c)+\frac{1}{2}x\phi''(c)(t-c)^2+\dots \right) dt \\
I_{1} & \approx f(c)e^{ x\phi(c) }\int_{c-\epsilon}^{c+\epsilon}e^{ x }\phi''(c)(t-c)^{2} / 2dt \\

\end{align}
$$
Set $s=[-x\phi''(c)]^{1/2}(t-c)$
$$
I_{1}\approx \frac{f(c)e^{ x\phi(c) }}{[-x\phi''(c)]^{1/2}}\int_{-[-x\phi''(c)]^{1/2}\epsilon}^{[-x\phi''(c)]^{1/2}\epsilon}e^{ -s^{2}/2 }ds
$$
$$
\begin{align}

I_{1} & \sim \frac{f(c)e^{x\phi(c)}}{[-x\phi''(c)]^{1/2}}\int_{-\infty}^{\infty}e^{ -s^{2}/2 }ds \\

I_{1} & \sim f(c)e^{x\phi(c)} \left( \frac{2\pi}{-x\phi''(c)} \right)^{1/2}
\end{align}
$$
Error induced by changing limits ? 
Recall $\int_{\xi}^{\infty}e^{-t^{2}/2}dt\sim \frac{1}{\xi}e^{-\xi^{2}/2}$ as $\xi\to \infty$
So error $\sim \frac{1}{[-x\phi''(c)]^{1/2}}\exp\left( -\frac{x^{2}\phi''(c)}{\lvert x\phi''(c) \rvert} \right)$
So error is exponentially small

So $I_{1}\gg I_{2}$ so $I\sim I_{1}$

### Example
$$
K_{0}(x)=\int_{0}^{\infty}\exp\left( -t-\frac{x^{2}}{4t} \right)dt
$$
Taking $\phi$