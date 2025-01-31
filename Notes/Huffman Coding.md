For simplicity, we take $a=\lvert \Sigma_{2} \rvert=2$
WLOG $p_{1}\geq p_{2}\geq\dots\geq p_{m}$
Huffman [[Code]] is defined inductively:
1. If $m=\lvert \Sigma_{1} \rvert=2$ assign codewords 0 and 1
2. If $m>2$, find a Huffman coding in the case of probabilities
$$
\begin{align}
 & \mu_{1},\mu_{2},\dots,\nu \\
 & p_{1},p_{2},\dots,p_{m-1}+p_{m}
\end{align}
$$
Append 0 (respectively 1) to the codewords for $\nu$ to give a codeword for $\mu_{m-1}$ (respectively $\mu_{m}$)

Note that this construction is prefix free.

### Theorem
Huffman codings are optimal.
#### Proof
##### Lemma 
Suppose $\mu_{1},\dots,\mu_{m}\in \Sigma_{1}$ are emitted with probabilities $p_{1},\dots,p_{m}$
Let $f$ be an [[Optimal Code]], prefix free, with word lengths $s_{1},\dots ,s_{m}$
1. If $p_{i}>p_{j}$ then $s_{i}\leq s_{j}$
2. There exist two codewords of maximal length which are equal up to the last digit.
###### Proof
1. If not, swap $i$th and $j$th codewords. This decreases the expected word length, contradicting optimality.
2. If not, then either there is only one code word of maximal length or any two codewords of maximal length differ before the last digit. In either case, delete the last digit of each codeword of maximal length. This maintains prefix-free condition, contradicting $f$ optimal.

#####
We show by 