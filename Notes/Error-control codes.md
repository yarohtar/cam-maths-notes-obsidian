WATCH LECTURE 5th OF FEBRUARY
[[Codewords]]
[[Binary Code]]
[[Information Rate]]

The information rate of $C$ is $\rho(C)=\frac{\log n}{n}$

We send a [[Binary Code]] through a [[Binary Symmetric Channel (BSC)]] making $n$ uses of the channel. Probability $p$ is the probability of a bit being mismatched.

Remark:
Soem convention needed in the case of a tie, eg. choose at random or ask for message to be sent again.
[[Decoding rules]]

[[Error detecting]]
[[Error correcting]]
[[Hamming distance]]
[[Minimum distance of a code]]
[[Asymptotic Equipartition Property]]
## New codes from old
[[Parity Extension]]
[[Punctured code]]
[[Shortened code]]
[[Perfect Code]]
[[Hamming's Bound]]
[[Gilbert-Shannon-Varshamov Bound]]
[[Size of Largest Code]]
[[Channel Capacity]]

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
by WLLN

### Proposition
The capacity of a [[Binary Symmetric Channel (BSC)]] with error probability $p<\frac{1}{4}$ is $\neq 0$

#### Proof
Choose $\nabl$