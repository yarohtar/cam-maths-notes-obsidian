Fix $\Sigma,V$ and $S\in V$.
1. A production rule $\alpha\to \beta$ is called noncontracting if $\lvert \alpha \rvert\leq \lvert \beta \rvert$
2. A production rule $A\to \beta$ is called context free if $A\in V$ and $\lvert \beta \rvert\geq1$
3. Production rules $A\to a$ and $A\to aB$ are called regular if $A,B\in V$ and $a\in \Sigma$
A [[Grammars]] is called respectively if all production rules satisfy a property above.
A [[Formal Language]] is called respectively if produced by a grammar of certain type.
Additionally:
Type 0: $\mathcal{L}(G)$ for any grammar $G$
Type 1: $\mathcal{L}(G)$ for noncontracting $G$
Type 2: $\mathcal{L}(G)$ for context-free $G$ 
Type 3: $\mathcal{L}(G)$ for regular $G$ 

[[Regular Formal Language]]