Let $X$ be a real or complex vector space. A norm of $X$ is a function $||\cdot||:X\to \mathbb{R}_{\geq 0}$ s.t.
1. $||x||=0 \iff x=0$
2. $||\lambda x||=|\lambda|\ ||x||$
3. $||x+y||\leq ||x||+||y||$
A normed space is a pair $(X,||\cdot||)$

NOTE: a normed space gives rise to a [[Metric spaces|metric space]] with $d(x,y)=||x-y||$. So we can talk about open sets, closed sets, convergent sequences etc.

[[L norms]]
[[Banach Space]]
[[Metric spaces#Some properties]]
[[Unit Ball]]

[[Separable Space]]

[[Equivalent Norms]]

[[Open Mapping Lemma]]

## New spaces from old 
For normed spaces $X$ and $Y$ can define a norm on $X\oplus Y$ by:
$\lVert (x,y) \rVert =\lVert x \rVert+\lVert y \rVert$
This space is written $X\oplus_{1}Y$

Similarly, have $X\oplus_{2}Y$ with $\lVert (x,y) \rVert=(\lVert x \rVert^2+\lVert y \rVert^2)^{1/2}$ 
And similarly for any $p$.

All are equivalent and all induce the product topology on $X\oplus Y$
Note that $X$ and $Y$ being [[Banach Space]] $\implies$ $X\oplus Y$ is Banach.
And also that $X$ and $Y$ are always closed subspaces of $X\oplus Y$

[[Quotients]]
[[Completions]]