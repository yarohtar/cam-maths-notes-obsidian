Let $X$ be a [[Well-ordering]] set and $Y$ be an arbitrary set.
Then for any [[Function]] $G:\mathcal{P}(X\times Y)\to Y$ there is unique $f:X\to Y$ such that
$$
\forall x\in X\quad %quad
f(x)=G(f|_{I_{x}})
$$
where $I_{x}$ is the [[Initial Segment]].

### Theorem
Say $h$ is an attempt if $h$ is a function $I\to Y$ where the domain of $h$ is an [[Initial Segment]] $I$ of $X$ and $\forall x\in dom(h)$, $h(x)=G(h|_{I_{x}})$
(Note that $I_{x}\subseteq dom(h)$)

The theorem says that there is a unique attempt whose domain is $X$ 

We first show that if $h,h'$ are attempts, then $h(x)=h'(x)$ for all $x\in dom(h)\cap dom(h')$ by induction.

Fix $$