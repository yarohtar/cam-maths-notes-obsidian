$S$ set, $R\subseteq F(S)$ where $F(S)$ is the [[Free Group]]. 
Let $\langle \langle R \rangle \rangle \unlhd F(S)$ be the smallest normal subgroup of $F(S)$ containing $R$ 
Define $\braket{ S | R }=F(S) /\langle \langle R \rangle \rangle$ group with generator $S$ and relative $R$ 
Data $(S,R)$ is called a presentation of the group (finite presentation if $S$ and $R$ are finite sets)

### Universal property of group presentations
For any group $H$, the function
$$
\begin{align}
\{ \text{gp hom }\braket{ S | R } \to H \} & \to \{\text{fn } S\to H \text{ st } \psi(r)=id_{H} \forall r\in R\} \\
\psi & \to \psi\circ pr\braket{ S | R } 

\end{align}
$$
Where 
$$
pr\braket{ S | R } :F(S)\to F(S) / \ll R\gg
$$
is bijective.
#### Proof
Suppose $\psi$, $\psi'$ give $\phi=\phi':S\to H$
By universal property of free groups,
$\psi\circ pr\braket{ S | R }=\psi'\circ pr\braket{ S | R }$
(Consider $F(S)\to \braket{ S | R }\to H$)
As $pr\braket{ S | R }$ surjective have $\psi=\psi'$.

Now assume $\phi:S\to H$ st the associated $\psi:F(S)\to H$ is st
$\psi(r)=id_{H}$ for all $r\in R$. Then $R\subseteq Ker(\psi)$
$Ker(\psi)\unlhd F(S)$, so $\ll R\gg \subseteq Ker(\psi)$ (by minimality)
$\psi$ descends to well defined $\bar\psi:F(S) / \ll R\gg\to H$

### Examples
$G=\braket{ t |  }\cong\mathbb{Z}$
$G=\braket{ a,b | ab^{-3},ba ^{-2} }\cong\mathbb{Z} /5$
