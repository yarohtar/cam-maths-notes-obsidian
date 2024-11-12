Let $E=E_{1}\times E_{2}$ with the [[Product measure]] $\mu$.
1. Let $f$ be a non-negative $\mathcal{E}$-[[Measurable Functions]]. 
   Then:
$$
\mu(f)=\int_{E_{1}}\left( \int_{E_{2}} f(x_{1},x_{2})\mu_{2}(dx_{2}) \right)\mu_{1}(dx_{1})
$$
2. Let $f$ be a $\mu$-integrable function. Define:
$$
A_{1}=\left\{  x_{1}\in E_{1}:\int_{E_{2}}\lvert f(x_{1},x_{2}) \rvert \mu_{2}(dx_{2}) <\infty \right\}
$$
and define $f_{1}:E_{1}\to \mathbb{R}$ by:
$$
f_{1}(x_{1})=\int_{E_{2}}f(x_{1},x_{2})
$$