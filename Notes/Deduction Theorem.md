Let $S\subseteq L$ and $p,q\in L$
Then $S\vdash(p \implies q)$ if and only if $S\cup \{ p \}\vdash q$

#### Proof
Assume $S\vdash(p \implies q)$. Write down the proof of $p \implies q$ from $S$ and add the following lines to obtain a proof of $q$ from $S\cup \{ p \}$:
$$
\begin{align}
p\quad %quad
\quad %quad
 & \text{(premis)} \\
q\quad %quad
\quad %quad
 & \text{(MP)}
\end{align}
$$

Now let's assume $S\cup \{ p \}\vdash q$. Let $t_{1},t_{2},\dots,t_{n}=q$ be a proof of $q$ from $S\cup \{ p \}$. We prove that $S\vdash(p \implies t_{i})$ by induction on $i$ 
1. $t_{i}$ 