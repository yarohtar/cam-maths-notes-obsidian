The operational channel capacity is the supremum over all [[Transmit Reliably|reliable transmission]] rates.

### Lemma
A [[Binary Symmetric Channel (BSC)]] with error probability $p<\frac{1}{4}$ has nonzero capacity.
#### Proof
Let $\delta$ be such that $2p<\delta<\frac{1}{2}$
We claim that we can [[Transmit Reliably]] at rate $R=1-H(\delta)>0$
Let $C_{n}$ have [[Size of Largest Code]] $\lvert C_{n} \rvert=A(n,\lfloor n\delta \rfloor)$
Then
$$
\lvert C_{n} \rvert \geq 2^{-n(1-H(\delta))} =2^{nR}
$$
Replacing $C_{n}$ with a subcode, we can assume $\lvert C_{n} \rvert=2^{nR}$
