$S$ set, $R\subseteq F(S)$ where $F(S)$ is the [[Free Group]]. 
Let $\langle \langle R \rangle \rangle \unlhd F(S)$ be the smallest normal subgroup of $F(S)$ containing $R$ 
$\braket{ S | R }=F(S) /\langle \langle R \rangle \rangle$ group with generator $S$ and relative $R$ 
Data $(S,R)$ is called a presentation of the group (finite presentation if $S$ and $R$ are finite sets)

### Universal property of group presentations
For any group $H$, the function
$$
\begin{align}
\{ \text{gp hom }\bar{\psi}:\braket{ S | R } \to H \} & \to \{\text{fn } \phi:S\to H \text{ st } \forall r\in R\ \psi(r)=e_{H} \} \\
\bar\psi & \to \bar\psi\circ pr\braket{ S | R } 

\end{align}
$$
is bijective. 
\*where 
$$
pr\braket{ S | R } :F(S)\to F(S) / \langle \langle R \rangle  \rangle 
$$
(Note that $\psi$ above is the natural homomorphism induced by $\phi$ in [[Free Group#Universal property of free groups]])

#### Proof
Suppose $\bar\psi$, $\bar\psi'$ give $\phi=\phi':S\to H$
By [[Free Group#Universal property of free groups|the universal property of free groups]],
$\psi\circ pr\braket{ S | R }=\psi'\circ pr\braket{ S | R }$
(Consider $F(S)\to_{pr} \braket{ S | R }\to_{\psi,\psi'} H$)
As $pr\braket{ S | R }$ surjective have $\psi=\psi'$.

Now assume $\phi:S\to H$ st the associated $\psi:F(S)\to H$ is st
$\psi(r)=id_{H}$ for all $r\in R$. Then $R\subseteq Ker(\psi)$
$Ker(\psi)\unlhd F(S)$, so $\langle \langle R \rangle \rangle\subseteq Ker(\psi)$ (by minimality)
$\psi$ descends to well defined $\bar\psi:F(S) / \langle \langle R \rangle \rangle\to H$

### Examples
$G=\braket{ t |  }\cong\mathbb{Z}$
$G=\braket{ a,b | ab^{-3},ba ^{-2} }\cong\mathbb{Z} /5$
