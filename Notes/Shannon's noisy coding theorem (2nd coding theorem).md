[[Operational Channel Capacity]] = [[Information Channel Capacity]]

### Proposition
For a [[Discrete Memoryless Channel (DMC)]] 
$$
\text{operational capacity }\leq \text{ information capacity}
$$
#### Proof
Let $C$ be the [[Information Channel Capacity]]. Suppose we can [[Transmit Reliably]] at rate $R>C$ i.e. there is a sequence of codes $(C_{n})_{n\geq 1}$ with $C_{n}$ of length $n$ and size $\lfloor 2^{nR} \rfloor$ s.t. $\hat{e}(C_{n})\to 0$.
The error probability defined as:
$$
e(C_{n})=\frac{1}{\lvert C_{n} \rvert }\sum_{c\in C_{n}}P(\text{error}|c \text{ sent})
$$
is clearly $e(C_{n})\leq \hat{e}(C_{n})$ (i.e. smaller than the max error probability)

Take random variable $X$ to be the input uniformly distributed over $C_{n}$, and $Y$ be the output when $X$ is transmitted and decoded. 
So, $e(C_{n})=P(X\neq Y)=p$ say
Then by [[Fano's Inequality]] write:
$$
\begin{align}
H(X|Y) & \leq H(p)+p\log(\lvert C_{n} \rvert-1) \\
 & 1+pnR \\
I(X;Y) & =H(X)-H(X|Y) \\
nC & \geq nR-1-(1+pnR) \\
pnR & \geq n(R-C)-2 \\
p & \geq \frac{n(R-C)-2}{nR}\not\to 0
\end{align}
$$
Thus the sequence of codes doesn't exist 

### Proposition
Consider a [[Binary Symmetric Channel (BSC)]] with error probability $p$. Let $R<1-H(p)$. Then there is a sequence of codes $(C_{n})_{n\geq 1}$ of length $n$ and size $\lfloor 2^{nR} \rfloor$ s.t. $e(C_{n})\to 0$ as $n\to \infty$
#### Proof
WLOG $p<\frac{1}{2}$ so there is some $\epsilon>0$ s.t. $R<1-H(p+\epsilon)$
We use [[Minimum Distance Decoding Rule]] (in case of tie pick arbitrary)
Let $m=\lfloor 2^{nR} \rfloor$
We pick an $[n,m]$ [[Binary Code]] $C$ at random 
(i.e. each with probability $\frac{1}{2^{n}\choose m}$) 
Say $C=\{ c_{1},\dots,c_{m} \}$
Choose $1\leq i\leq m$ at random (i.e. each with probability $\frac{1}{m}$) 
We send $c_{i}$ through the channel and get output $Y$ 

It suffices to show 
$$
P(Y\text{ is not detected as }c_{i})\to 0
$$
Let $r=\lfloor n(p+\epsilon) \rfloor$
$$
\begin{gather}
P(Y\text{ is not detected as }c_{i}) \\
\quad %quad
\quad %quad
\leq P(c_{i}\not\in B(Y,r))+P(B(Y,r)\cap C\supset \{ c_{1} \})
\end{gather}
$$