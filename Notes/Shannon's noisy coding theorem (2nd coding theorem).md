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
