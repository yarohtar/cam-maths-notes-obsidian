$S=\{ s_{\alpha} \}_{\alpha \in I}$ set "alphabet"
$S^{-1}=\{ s_{\alpha}^{-1} \}_{\alpha \in I}$ also set of symbols (this is just a label, its not an actual inverse ~~yet~~)
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
- If $(s_{\alpha_{1}}^{\epsilon_{1}}\dots,s_{\alpha_{n}}^{\epsilon_{n}})$ is not reduced: say it contains subword $(s_{\alpha},s_{\alpha}^{-1})$ then the image contains $\phi(s_{\alpha})\phi(s_{\alpha})^{-1}=e_{H}$
  So if two words related by element reduction, then $\psi$ has the same image
- Group operation on $F(S)$ is concatenat+reduct, so $\psi$ is homomorphism

[[Group Presentation]]
## Free products with amalgamation
$G_{1},G_{2}$, $G_{i}=\braket{ S_{i} | R_{i} }$ with $S_{1}\cap S_{2=\emptyset}$
Free product of $G_{1}$ and $G_{2}$: $G_{1}*G_{2}=\braket{ S_{1}\cup S_{2} | R_{1}\cup R_{2} }$
universal property gives $j_{i}:G_{i}\to G_{1}*G_{2}$

Suppose also $H$ is a group $i_{1}:H\to G_{1}$ and $i_{2}:H\to G_{2}$ group hom

Free product with amalgamation over $H$:
$$
G_{1}*_{H}G_{2}=G_{1}*G_{2} /\langle \braket{ (j_{1}i_{1}(h))(j_{2}i_{2}h)^{-1} | h\in H }  \rangle 
$$
Induced maps also called $j_{i}:G_{i}\to G_{1}*_{H}G_{2}$

### Universal property of amalgamated free products
For any group $K$, the function from gp homs $G_{1}*_{H}G_{2}\to K$ to group homs $\phi_{1}:G_{1}\to K$ and $\phi_{2}:G_{2}\to K$ st $\phi_{1}\circ i_{1}=\phi_{2}\circ i_{2}$ 
that sends $\psi$ to $(\phi_{1}=\psi \circ j_{1},\phi_{2}=\psi \circ j_{2})$
is bijective.
#### Proof
Just expand the definitions ... umm yea 