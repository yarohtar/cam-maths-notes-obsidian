$S=\{ s_{\alpha} \}_{\alpha \in I}$ set "alphabet"
$S^{-1}=\{ s_{\alpha}^{-1} \}_{\alpha \in I}$ also set of symbols (this is just a label, its not an actual inverse)
$S\cap S^{-1}=\emptyset$
Word in the alphabet $S$ finite sequence $(x_{1},x_{2},\dots,x_{n})$
A word is reduced if it has no subwords of form $(s_{\alpha},s_{\alpha}^{-1})$ or $(s_{\alpha}^{-1},s_{\alpha})$
Elementary reduction of a word
Replace $(x_{1},\dots,x_{i},s_{\alpha},s_{\alpha}^{-1},x_{i+3},\dots x_{n})$ with $(x_{1},\dots,x_{i},x_{i+3},\dots ,x_{n})$
Similarly for $s_{\alpha}^{-1},s_{a}$

Define $F(s)$ the free group on the alphabet $S$, the set of reduced words in $S$ (including $\emptyset=()$). Group operation: concatenate words
then apply elementary reductions iteratively.

well defined and associative in handout ! (also ORW notes)

Let $i:S\to F(S)$ with $s_{\alpha}\to(s_{\alpha})$
### Universal property of free groups
For any group $H$, the function:
$$
\begin{align}
\{ \text{gp hom } F(S)\to H \} & \to \{ \text{functions }\phi:S\to H \} \\
\psi & \to \psi\circ i

\end{align}
$$
is a bijection

#### Proof
Given $\phi:S\to H$ set 
$$
\psi((s_{\alpha_{1}}^{\epsilon_{1}},\dots s_{\alpha _{n}}^{\epsilon_{n}}))=\phi(s_{\alpha_{1}})^{\epsilon_{1}}\dots \phi(s_{\alpha_{n}})^{\epsilon_{n}}
$$
