From a complicated function $f(x)$, we want to find a simpler $g(x)$ s.t. $f\sim g$. 
Want to break up $g$ into a hierarchy of approximations s.t.
$$g(x)=\sum_{k=0}^{N} a_{k}\phi_{k}(x)$$
where $\phi_{k}(x)$ are very simple and relative sizes of $\phi_{k}$ are known.

### Definition
Suppose we have an [[Asymptotic Approximation]] which holds for all $N$. Then we have an asymptotic series and we write:
$$
f(x)\sim \sum_{k=0}^{\infty} a_{k}\phi_{k}(x)
$$
We make NO CLAIMS about this converging !!!!
We never fix $x$ and let $N\to \infty$.
### Properties
Let $f\sim \sum a_{k}\phi_{k}$ and $g\sim \sum b_{k}\phi_{k}$
- Linearity: $\alpha f$
- Consider $\phi_{k}=(x-a)^k$