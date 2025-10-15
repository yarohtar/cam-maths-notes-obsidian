An isomorphism in a [[Category]] $\mathcal{C}$ is a [[Morphism]]
$$
f:A\to B
$$
such that there is a morphism (called the inverse)
$$
g:B\to A
$$
and both of the following hold:
$$
fg=1_{B}
$$
$$
gf=1_{A}
$$
### Lemma
Suppose $f$ is an isomorphism with inverse $f^{-1}$.
Suppose $fg=1_{B}$ and/or $hf=1_{A}$ for some $B\xrightarrow{g,h}A$.
Then
$$
g=f^{-1}\quad %quad
 \text{and/or}\quad %quad
 h=f^{-1}
$$
#### Proof
Suppose $fg=1_{B}$
Compose with $f^{-1}$ on the left:
$$
f^{-1}(fg)=f^{-1}1_{B}
$$
Use [[Associativity]]
$$
(f^{-1}f)g=f^{-1}1_{B}
$$
By definition of $f^{-1}$, we have $f^{-1}f=1_{A}$
$$
1_{A}g=f^{-1}1_{B}
$$
By definition of identities:
$$
g=f^{-1}
$$