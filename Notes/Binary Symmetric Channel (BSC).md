[[Discrete Memoryless Channel (DMC)]] which has $\Sigma_{1}=\Sigma_{2}=\{ 0,1 \}$ with probability $0\leq p\leq 1$ and [[Channel Matrix]]
$$
\begin{pmatrix}
1-p & p \\
p & 1-p
\end{pmatrix}
$$
ie $p$ is probability a symbol is mistransmitted.

### Lemma
Let $\epsilon>0$. A [[Binary Symmetric Channel (BSC)]] with error probability $p$ is used to send $n$ digits. Then
$$
P(\text{BSC makes }\geq n(p+\epsilon) \text{ errors})\to 0
$$
as $n\to \infty$
#### Proof
Let 
$$
\mu_{i}=\begin{cases}
1 & \text{if }i\text{th digit is mistransmitted} \\
0 & \text{otherwise}
\end{cases}
$$
$\mu_{1},\mu_{2},\dots$ are iid variables
$$
\begin{align}
P(\text{BSC makes }\geq n(p+\epsilon)\text{ errors}) & =P\left( \sum \mu_{i}\geq n(p+\epsilon) \right) \\
 & \leq P\left( \left\lvert  \frac{1}{n}\sum \mu_{i}-p  \right\rvert \geq \epsilon \right)\to 0
\end{align}
$$
by weak law of large numbers.