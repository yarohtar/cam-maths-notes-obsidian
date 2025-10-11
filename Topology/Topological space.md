Let $X$ be a set. Topology $\tau$ is a collection of subsets of $X$ s.t.
- $\emptyset\in \tau$ and $X\in \tau$
- $\forall i \in I, U_i\in \tau\implies U_{i\in I}\in \tau$
- $U,V\in \tau\implies U\cap V\in\tau$
A topological space is the pair $(X,\tau)$.
Members of $\tau$ are called open sets of $X$.
A subset of $X$ is closed if its complement is open.

### Examples
- Indiscrete topology $\tau=\{\emptyset, X\}$ (not induced by any metric)
- Discrete topology $\tau=2^X$ (induced by discrete metric)
- Cofinite topology of all sets whose complement is finite
- Cocountable topology of all sets whose complement is countable


## Basic properties/defns
1. Some topologies are induced by a [[Metric space|metric]].
2. [[Hausdorff]]
3. $A\subset X$ is open if every point has an open [[Neighbourhood|nbd]] that is contained in $A$
4. $x_n\to x$ if for any nbd $V$ of $x$ we find $N$ s.t. $x_n\in V$ for $n>N$
5. In a [[Hausdorff]], the limits are unique.
6. Suppose $A\subset X$ is closed and $x_n\to x$ in $X$ and $x\not\in A$. Then no open nbd of $x$ is in $X\setminus A$ but then $X\setminus A$ is not open contradiction so it has to be $x\in A$.
7. HOWEVER, a set $A$ which contains all its limit points no longer has to be closed.
8. [[Accumulation points]]
9. [[Interior and closure]]
10. [[Subspace topology]]
11. [[Continuity in topological spaces]]
12. $X$ and $Y$ are [[Homeomorphism|homeomorphic]] if there is a bijection $f$ between them such that both $f$ and $f^{-1}$ are continuous
13. [[Product topology]]
14. [[Open map]]
15. [[Quotient space]]

## More stuff
[[Connectedness]]
[[Compactness]]
[[Sequential compactness]]