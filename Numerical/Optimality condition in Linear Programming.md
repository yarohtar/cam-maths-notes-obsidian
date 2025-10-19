Consider a [[Linear Program]] in the standard form:
" Minimize $c^Tx$ over $x\in \mathbb{R}^{n}$ subject to $Ax=b$ and $x\geq 0$ "
where the matrix $A\in \mathbb{R}^{m\times n}$ has rank $m$
and $c\in \mathbb{R}^{n},\ b\in \mathbb{R}^{m}$ are vectors.
Suppose $x$ is a [[Basic Feasible Solution]] with [[Basis]] $B\subseteq[n]$
Suppose also that:
$$
c-A^{T}((A^{T}_{B})^{-1}c_{B})\geq0
$$
Then $x$ is optimal.
Moreover, there exists a [[Basis]] $B\subseteq[n]$ such that:
$$
c-A^{T}((A^{T}_{B})^{-1}c_{B})\geq 0
$$
and $\lambda=(A_{B}^{T})^{-1}c_{B}$ is then the optimal solution to the 
[[Dual Problem in Linear Programs]]:
" Maximize $\lambda^{T}b$ over $\lambda \in \mathbb{R}^{m}$ subject to $A^{T}\lambda\leq c$ "

We present the proof through several lemmata.
### Lemma
Let $A\subseteq \mathbb{R}^{m\times n}$ have rank $m$
Let $f:\mathbb{R}^{m}\to \mathbb{R}$ defined by:
$$
f(b)=\min \{ c^{T}x : Ax=b,\ x\geq 0 \}
$$
Let $b\in \mathbb{R}^{m}$ and suppose $f(b)$ achieves its minimum.
Then there is some [[Basis]] $B\subseteq[n]$ of $A$
such that the unique [[Basic Feasible Solution]] $x\in \mathbb{R}^{n}$ to $Ax=b$
with [[Basis]] $B$ has the following property:
Let $s \in \mathbb{R}^{n}$ be such that $s\geq0$ and [[Support]] of $s$ is a subset of $B$.
Let $g(t)=f(b+tAs)$
Then there is some $t>0$ such that $g(t)=c^{T}(x+ts)$.
#### Proof
For $\epsilon>0$ small enough, define $x:[0,\epsilon]\to \mathbb{R}^{n}$ satisfying:
- $x(0)=x$
- $x(t)$ is a [[Basic Feasible Solution]] for $Ax(t)=b+tAs$
- $f(b+tAs)=c^{T}x(t)$
Note that $x+ts$ is a [[Basic Feasible Solution]] for $A(x+ts)=b+tAs$
when $t$ is small enough.
So $f(b+tAs)$ does achieve its minimum somewhere
and thus it achieves its minimum at some [[Basic Feasible Solution]].

Now assume that $f(b+tAs)< c^{T}(x+ts)$ for all small enough $t$
Let $B(t)$ be a [[Basis]] for $x(t)$
There is only $\binom{ n }{ m }$ choices for $B(t)$ 
so one of them appears infinitely often.
Denote this [[Basis]] by $B_{\infty}$
Take a sequence $t_{n}\to 0$
such that $B_{\infty}$ is the [[Basis]] of $x(t_{n})$
Then 
$$
x(t_{n})_{B_{\infty}} = A_{B_{\infty}}^{-1} (b+ t_{n}As)
$$
RHS clearly converges to $A_{B_{\infty}}^{-1}b$ as $n\to \infty$ 
so $x(t_{n})$ converges to some $x'$ 
where $x'_{B_{\infty}}=A_{B_{\infty}}^{-1}b$ and $x'_{i}=0$ for $i\not\in B_{\infty}$
Then also $g(t_{n})=c^{T}x(t_{n})$ converges to $c^{T}x'$
By properties of the limits, $c^{T}x'\leq c^{T}x=g(0)$
By choice of $g()$




Let $t>0$ be small and $x(t)$ a [[Basic Feasible Solution]] for $Ax(t)=b+tAs$
such that $f(b+tAs)=c^{T}x(t)$.
Note that this is always defined for small $t$
because in particular $x+ts$ is a [[Basic Feasible Solution]] for 
$$
A(x+ts)=b+tAs
$$
so $f(b+tAs)$ does achieve its minimum somewhere 
and thus it achieves it at some [[Basic Feasible Solution]].
If for all small enough $t>0$ we have $c^{T}x(t)=c^{T}(x+ts)$ then we are done.
If for any $n$ we had $x(t_{n})-t_{n}s\geq 0$ 
then we would find 
$$
f(b)\leq c^{T}x(t_{n})-t_{n}c^{T}s<c^{T}x
$$
which is a contradiction.
Thus for every $n$ there is some index $i_n$ such that
$$
x(t_{n})_{i_{n}} - t_{n} s_{i_{n}} <0
$$
But as we know $x(t_{n})\geq 0$ and $t_{n}\to 0$
it has to be that for large $n$ we have 



Firstly, let $X(b)$ be the set of [[Basic Feasible Solution]]s 
By definition of [[Basis]], we have that $A_{B}$ is invertible.
Thus form the vector $s'\in \mathbb{R}^{n}$ 
by $s_{B}'=A_{B}^{-1}s$ and $s_{i}'=0$ for $i\not\in B$

For small enough $\epsilon>0$ and all $0\leq t\leq\epsilon$
we have that $A(x+t s')=b$ and $x+ts'\geq 0$.
Notably, $x+ts'$ is still a [[Basic Feasible Solution]].
Thus
$$
f(b+ts) \leq c^{T}(x+ts')=f(b) + t c^{T}s'
$$
Suppose $f(b+t_{1}s)<f(b)+t_{1}c^{T}s'$ for some $0<t_{1}\leq \epsilon$
Now let $x_{1}$ be a [[Basic Feasible Solution]] such that:
$$
f(b+t_{1}s) = c^{T}x_{1}
$$
Define $s_{1}'$ similarly to $s'$ above,
and note that for small enough $\delta>0$ and all $0\leq k\leq \delta$:
$$
f(b+t_{1}s-ks) \leq c^{T}x_{1} - kc^{T}s_{1}' \leq f(b) + c^{T} (ts'-ks_{1}')
$$
and on the other side:
$$

$$

Let $s \in \mathbb{R}^{m}$ and $\epsilon>0$
Suppose $f(b)=c^{T}x$ for some $x$ such that $Ax=b$.
We can WLOG assume that $x$ is a [[Basic Feasible Solution]].
Thus $x$ has a [[Basis]] $B\subseteq[n]$ where $A_{B}$ is invertible.
Define $s'\in \mathbb{R}^{n}$ by $s'_{B}=A_{B}^{-1}s$ and $s'_{i}=0$ for $i\not\in B$
Define $x'=x+\epsilon s'$
Now $f(b+\epsilon s)\leq c^{T}x' = f(b)+\epsilon c^{T}s'$
Similarly, if $x_{1}$ is such that $f(b+\epsilon s)=c^{T}x_{1}$
then $f(b)\leq f(b+\epsilon s)-\epsilon c^{T}s'$

### Lemma
Consider a [[Linear Program]]:
" Minimize $c^Tx$ over $x\in \mathbb{R}^{n}$ subject to $Ax=b$ and $x\geq 0$ "
where $A\in \mathbb{R}^{m\times n}$, $c\in \mathbb{R}^{n}$ and $b\in \mathbb{R}^{m}$.
Suppose $x$ is a [[Basic Feasible Solution]] with [[Support]] $S\subseteq[n]$
Then $x$ is optimal
if and only if
$$
c - A^{T}\lambda \geq 0
$$
for some $\lambda \in \mathbb{R}^{m}$ satisfying $(A_{S}^{T})\lambda=c_{S}$
where $A_{S}$ is $m\times \lvert S \rvert$ submatrix of $A$
obtained by taking $i$-th columns of $A$ for all $i\in S$

Moreover, $\lambda$ is then feasible and optimal solution 
for the [[Dual Problem in Linear Programs]]:
" Maximize $\lambda^{T}b$ over $\lambda \in \mathbb{R}^{m}$ subject to $A^{T}\lambda\leq c$ "
### Proof
Start from the [[Dual Problem in Linear Programs]]:
" Maximize $\lambda^Tb$ over $\lambda \in \mathbb{R}^{m}$ subject to $A^{T}\lambda\leq c$ "
Note that a feasible $x$ is primal optimal 
and feasible $\lambda$ is dual optimal
if and only if 
[[Complimentary Slackness]] holds (due to [[Dual Problem in Linear Programs#Lemma]])
i.e. $x^{T}(c-A^{T}\lambda)=0$
i.e. $c_{S} - A_{S}^{T}\lambda=0$ (due to [[Support]] of $x$ being $S$)
#### $\implies$
Suppose $x$ is primal optimal.
By [[Strong duality in linear programs]], 
there is some feasible $\lambda$ that is dual optimal.
By the observation above, this means 
$$
c_{S}-A_{S}^{T}\lambda=0
$$
By feasibility of $\lambda$:
$$
c-A^{T}\lambda\geq 0
$$
#### $\impliedby$
Suppose some $\lambda$ satisfying $(A_{S}^{T})\lambda=c_{S}$ also satisfies:
$$
c-A^{T}\lambda\geq 0
$$
Then $\lambda$ is feasible, and $(c-A^{T}\lambda)x=0$ so [[Complimentary Slackness]] holds.
This happens if and only if $x$ is primal optimal and $\lambda$ is dual optimal.

### Lemma
Let $x$ be a [[Basic Feasible Solution]] with [[Support]] $B\subseteq[n]$
and suppose $\lvert B \rvert=m$ (i.e. $B$ is a [[Basis]] of $x$)
Then $x$ is optimal 
if and only if
$$
c-A^{T}((A_{B}^{T})^{-1}c_{B})\geq 0
$$
### Proof
Using the previous theorem, 
the unique $\lambda \in \mathbb{R}^{m}$ satisfying $(A_{B}^{T})\lambda=c_{B}$ is exactly:
$$
\lambda=(A_{B}^{T})^{-1}c_{B}
$$
where we used the fact that $A_{B}$ is square (due to $\lvert B \rvert=m$)
and invertible by the definition of [[Basic Solution]].

## Proof

