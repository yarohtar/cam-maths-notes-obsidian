Let $(\Omega,\mathcal{P},\mathbb{P})$ be a [[Probability Space]]
Let $A$ be a discreet set.
Let $X:\Omega \to A$ be a [[Random Variable]] 
Let $P:A\to[0,1]$ be given by:
$$
P(a) = \mathbb{P}(X=a)
$$
i.e. the distribution of $X$.
Consider now the [[Random Variable]] $Q:\Omega\to[0,1]$ given by:
$$
Q(\omega) = P(X(\omega))
$$
often written as just $Q=P(X)$.
From the definition of $P$, 
you might naively substitute:
$$
Q=P(X)=\mathbb{P}(X=X)=1
$$
This is wrong. 
We need to fully expand the definitions to understand why:
$$
Q=P(X)=\mathbb{P}(\{ \omega \in \Omega : X(\omega) = X \})
$$
