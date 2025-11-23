We say that $\phi:\mathbb{N}\to \Omega$ corresponds to $\iota \in \Omega$ if $\lvert \iota-\phi(n) \rvert\leq2^{-n}$ for all $n\in \mathbb{N}$.
We say that $\phi:\mathbb{N}\to \Omega$ and $\phi':\mathbb{N}\to \Omega$ agree until $n$ if $\phi(k)=\phi'(k)$ for all $k\leq n$.

Suppose $\phi_{0}:\mathbb{N}\to \Omega$ is computable, corresponding to some $\iota_{0}\in \Omega$.
Furthermore, suppose $\phi_{m}:\mathbb{N}\to \Omega$ are computable for $m\in \mathbb{N}$,
and correspond to some $\iota_{m}\in \Omega$.
Suppose that $\lim_{m\to \infty}\iota_{m}=\iota_{0}$.

Finally, suppose that there is a computable $I:\mathbb{N}\to \mathbb{N}$ such that $I(n)=\text{code}(\phi_{n})$ for all $n\geq 0$.

Now let $f:\Omega \to?$ be computable in the following sense:
There is some computable $\Gamma:\mathbb{N}\to?$ such that whenever $n$ is a code for some computable $\phi:\mathbb{N}\to \Omega$, and $\phi$ corresponds to some $\iota \in \Omega$, then $\Gamma(n)=f(\iota)$.

Now let $\phi_{0}$ correspond to $\iota_{0}$.
Then there is some $n$ such that for any $\phi'$ that agrees with $\phi_{0}$ until $n$ we have $\Gamma(\text{code}(\phi_{0}))=\Gamma(\text{code}(\phi'))$.



Let $\Gamma:\mathbb{N} \to ?$ be any algorithm with the following property:
For any $\iota \in \Omega$, suppose that $n$ and $n'$ are codes for some $\phi$ and $\phi'$ which both correspond to $\iota$.
Then $\Gamma(n)=\Gamma(n')$.



Let $\iota_{0}\in \Omega$, and let $\{ \iota_{m} \}_{m>0}\in \Omega^{\mathbb{N}}$ such that $\lvert \iota_{m}-\iota_{0} \rvert<2^{-m}$
Let $\Omega_{C}$ be the set of all computable functions $\phi:\mathbb{N}\to \Omega$ 
such that there is some $\iota \in \Omega$ and $\lvert \phi(n)-\iota \rvert<2^{-n}$ for all $n\in \mathbb{N}$.
(i.e. $\Omega_{C}$ is the set of codes for elements of $\Omega$).

Suppose that $\Gamma:\Omega_{C} \to M$ is computable and has the following property:
Fix $\iota \in \Omega$.
Then for any computable $\phi:\mathbb{N}\to \Omega$ such that $\lvert \phi(n) - \iota \rvert<2^{-n}$
we have that $\Gamma(\phi)$ is fixed.
