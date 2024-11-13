A regular formal language or a Type 3 language ([[The Chomsky Hierarchy]]) is produced by rules $A\to a$ and $A\to aB$ where $A,B$ are variables and $a$ is a termination symbol. ([[Grammar]])
### Proposition
If $G,G'$ are regular grammars and $V\cap V'=\emptyset$, then 
1. If $H$ [[Regular Concatenation Grammar|RCG]], then $\mathcal{L}(H)=\mathcal{L}(G)\mathcal{L}(G')$
2. If $H$ [[Regular Union Grammar|RUG]], then $\mathcal{L}(H)=\mathcal{L}(G)\cup \mathcal{L}(G')$

### Theorem
TFAE:
1. $L$ is regular
2. $L=\mathcal{L}(D)$ for $D$ [[Deterministic Automata]]
3. $L=\mathcal{L}(N)$ for $N$ [[Nondeterministic Automata]]

### Lemma
[[Regular Pumping Lemma]]