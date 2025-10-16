Given finite sets $A$ and $B$:
$$
\lvert A\cup B \rvert =\lvert A \rvert  + \lvert B \rvert  - \lvert A\cap B \rvert 
$$
Moreover, given finite sets $A_{1},A_{2},\dots,A_{n}$:
$$
\left\lvert  \bigcup_{i=1}^{n} A_{i}  \right\rvert  = \sum_{k=1}^{n} (-1)^{k+1} \sum_{1\leq i_{1}< \dots < i_{k} \leq n} \left\lvert  \bigcap_{j=1}^{k} A_{i_{j}}  \right\rvert 
$$
or equivalently:
$$
\left\lvert  \bigcup_{i=1}^{n} A_{i}  \right\rvert = \sum_{S\subseteq[n]} (-1)^{\lvert S \rvert +1} \left\lvert  \bigcap_{i\in S} A_{i}  \right\rvert 
$$
where $[n]=\{ 1,\dots,n \}$ and we take empty intersection to be empty.

By taking complements with respect to $A=\bigcup_{i=1}^{n}A_{i}$:
$$
\left\lvert  \overline{\bigcap_{i=1}^{n} A_{i}}  \right\rvert =\sum_{S\subseteq[n]} (-1)^{\lvert S \rvert +1} \left\lvert \overline{ \bigcup_{i\in S} A_{i}}  \right\rvert 
$$
$$
\lvert A \rvert - \lvert  \rvert 
$$