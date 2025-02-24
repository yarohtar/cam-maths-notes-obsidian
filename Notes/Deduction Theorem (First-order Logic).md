Let $S$ be a set of formulae in a first-order language $L$. Let $p$, $q$ be formulae in $L$. Then $S\vdash p\implies q$ if and only if $S\cup \{ p \}\vdash q$
### Proof
Assume $S\vdash(p\implies q)$. Write down a proof of $(p\implies q)$ from $S$ and add the lines 
$$
\begin{align}
p\quad %quad
\quad %quad
 & \text{(premiss)}  \\
q\quad %quad
\quad %quad
 & \text{(MP)}
\end{align}
$$
to obtain a proof of $q$ from $S\cup \{ p \}$

Now assume $S\cup \{ p \}\vdash q$. Let $t_{1},\dots,t_{n}$ be a proof of $q$ from $S\cup \{ p \}$
We prove by induction on $i$ that $S\vdash(p\implies t_{i})$
Induction hypothesis at $i$th step:
For all $j<i$ we have $S\vdash(p\implies t_{j})$ s.t. if a variable $x$ does not occur free in any premiss in the proof $t_{1},\dots,t_{j}$ of $t_{j}$ from $S\cup \{ p \}$ 
then $x$ must not occur free in any premiss used in the proof of $(p\implies t_{j})$ from $S$.
