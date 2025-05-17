The information rate $H$ of a [[Source]] is the infimum of all rates at which it is [[Reliably encodable]]
### Lemma
The [[Source Information Rate]] of a [[Bernoulli Source]] is at most the expected word length of an [[Optimal Code]].
![[Pasted image 20250517175119.png]]
#### Proof
Let $c$ be an optimal code
Let $s_{1},s_{2},\dots$ be codeword lengths when we encode $X_{1},X_{2},\dots$
Let $\epsilon>0$
Let 
$$
A_{n}=\{ x : c^{*}(x) \text{ has length less than }n(\mathbb{E}(s_{1})+\epsilon) \}
$$
Then
$$
\begin{align}
\mathbb{P}((X_{1},\dots,X_{n})\in A_{n})  &  = \mathbb{P}\left( \sum_{i=1}^{n}s_{i}\leq n(\mathbb{E}(s_{1})+\epsilon) \right) \\
 & =\mathbb{P}\left( \left\lvert  \frac{1}{n}\sum_{i=1}^{n}s_{i}-\mathbb{E}(s_{i})  \right\rvert <\epsilon \right) \\
 & \to 1 
\end{align}
$$
Now $c^{*}$ is injective, hence $\lvert A_{n} \rvert\leq 2^{n(\mathbb{E}(s_{1})+\epsilon)}$. 
Making $A_{n}$ larger if necessary, we can assume $\lvert A_{n} \rvert=\lfloor 2^{n(\mathbb{E}(s_{i})+\epsilon)} \rfloor$
Taking logarithms 
$$
\frac{\log \lvert A_{n} \rvert }{n}\to \mathbb{E}(s_{1})+\epsilon
$$
So the source is reliably encodable at rate $r=\mathbb{E}(s_{1})+\epsilon$ for all $\epsilon>0$. Hence the information rate is at most $\mathbb{E}(s_{1})$
### Corollary
A Bernoulli source has information rate less than $H(X)+1$.
#### Proof
[[Shannon's noiseless coding theorem]]
### Proposition
The information rate $H$ of a Bernoulli source is at most $H(X)$. 
#### Proof
Encode $X_{1},X_{2},\dots$ in blocks of size $N$. Let $Y_{1}=(X_{1},\dots,X_{N})$ etc. 
Then if $X$ has information rate $H$, $Y$ has information rate $NH$
Apply the previous corollary:
$$
NH<H(Y)+1=H(X_{1},\dots,X_{N})+1=NH(X)+1
$$
to find $H<H(X)+\frac{1}{N}$ so $H\leq H(X)$.