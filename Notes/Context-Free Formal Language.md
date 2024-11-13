A context-free formal language or a Type 2 language ([[The Chomsky Hierarchy]]) is produced by the rules $A\to \alpha$ where $A$ is a variable, and $\lvert \alpha \rvert\geq 1$. ([[Grammar]])

### Proposition
For a context free grammar $G$ and any word $w\in \mathcal{L}(G)$ there is a (not necessarily unique) [[Parse Tree]] $T$ such that $\sigma_{T}=w$.

### Theorem
Every context free grammar $G$ has a [[Chomsky Normal Form]] grammar $G'$ such that $\mathcal{L}(G)=\mathcal{L}(G')$
#### Proof (sketch)
The product rules we need to kick out are:
1. Unit producions $A\to B$
2. bad productions $A\to \alpha$ where $\alpha \in V^*$ but $\lvert \alpha \rvert>2$
3. very bad productions $A\to \alpha$ where $\lvert \alpha \rvert\geq 2$ but $\alpha$ contains terminal symbols.
First kick the very bad productions out easily. 
Then add unit closure rules (for every $A\to B$ and $B\to \alpha$ add rule $A\to \alpha$) and prove that removing unit productions from a unit closed grammar doesn't change the language.
