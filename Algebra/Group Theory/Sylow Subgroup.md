Let $p$ be prime and $G$ a finite [[Group]] of order $p^am$ where $p \nmid m$. 
A Sylow $p$-subgroup of $G$ is $P\leq G$ s.t. $|P|=p^a$. 
[[Groups of prime order]]
The set of Sylow $p$-subgroups is denoted by $Syl_p(G)=\{P\leq G: |P|=p^a\}$. 
[[First Sylow Theorem]]
[[Second Sylow Theorem]]
[[Third Sylow Theorem]]
### Third Sylow Theorem
The number $n_p=|Syl_p(G)|$ satisfies $n_p\equiv 1\pmod{p}$ and $n_p\mid m$.
#### Proof
By the second Sylow theorem, $G$ acts transitively on $Syl_p(G)$, 
so $n_p\mid |G|$ so it suffices to show $n_p\equiv 1\pmod p$. 
Let $P$ be a Sylow $p$-subgroup. 
Consider the conjugacy action of $P$ on $Syl_p(G)$. 
Note that all orbits of this action are divisors of $|P|=p^a$. 
Also $Orb_P(P)=\{P\}$. 
Suppose another orbit has order 1, i.e. orbit of $Q$ is of size 1. 
Then $P\leq N_G(Q)$, so $P$ and $Q$ are Sylow $p$-subgroups of $N_G(Q)$. 
So for some $g\in N_G(Q)$ we have $P=gQg^{-1}=Q$. 
Hence there is exactly one orbit of size $1$, 
but $n_p$ is the sum of orbit sizes so it has to be $n_p\equiv 1\pmod p$.
### Corollary
If $n_p=1$ then there is a normal Sylow $p$-subgroup of $G$.
#### Proof
$Syl_p(G)$ is closed under conjugation.
