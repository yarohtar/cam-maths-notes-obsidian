Fix $\Sigma$. $D=(\Sigma,Q,\delta,q_{0},F)$ is called a deterministic automata if 
1. $Q$ is a finite set of states
2. $q_{0}\in Q$ is a start state
3. $F\subseteq Q-\{ q_{0} \}$ accept states
4. $\delta:Q\times \Sigma\to Q$ transition function

### Interpretation
1. Get a word $w\in \mathbb{W}$ as input
2. Start at state $q_{0}$
3. Read the word letter by letter: 
   If you're in state $q$ and read $a$, move to $\delta(q,a)$
4. After reading all of $w$, you're in some state $q$:
   If $q\in F$ then $D$ ACCEPTS $w$.
   If $q\not\in F$ then $D$ REJECTS $w$.
