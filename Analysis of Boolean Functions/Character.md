Let $G$ be a finite [[Abelian]] [[Group]].
A character on $G$ is a [[Homomorphism]] 
$$
\chi:G\to \mathbb{T}=\{ z\in \mathbb{C}:\lvert z \rvert =1 \}
$$

## Theorem
The characters on $G$ form an [[Orthonormal Basis]] of $\mathbb{C}^{G}$
### Proof
Let $\chi_{1}$ and $\chi_{2}$ be characters and $\chi=\chi_{1}\overline{\chi_{2}}$.
If $\chi_{1}=\chi_{2}$ then clearly $\mathbb{E}_{x}\chi = 1$.
Otherwise pick some $u$ such that $\chi(u)\neq 1$ and note:
$$
\mathop{\Large\mathbb{E}}\limits_{x\in G}\chi(x) = \mathop{\Large\mathbb{E}}\limits_{x\in G} \chi(ux) = \chi(u)\mathop{\Large\mathbb{E}}\limits_{x\in G}\chi(x)
$$
and thus $\mathbb{E}_{x}\chi(x)=0$.

It remains to prove that they span $\mathbb{C}^{G}$.
As $G$ is a [[Finite Abelian Group]], write
$$
G=\mathbb{Z} / m_{1}\mathbb{Z} \times \mathbb{Z} / m_{2} \mathbb{Z} \times \dots \times \mathbb{Z} / m_{n} \mathbb{Z}
$$
Given $r,x\in G$ where $r=(r_{1},\dots,r_{n})$ and $x=(x_{1},\dots x_{n})$ let
$$
\chi_{r}(x) = \prod_{j=1}^{n} e^{2\pi i \\frac{  }{  }}
$$


## Corollary
The size of the [[Pontryagin Dual]] is smaller than the size of $G$.
For the reverse result use [[Finite Abelian Group]].
