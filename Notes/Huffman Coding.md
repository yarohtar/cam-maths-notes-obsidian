For simplicity, we take $a=\lvert \Sigma_{2} \rvert=2$
WLOG $p_{1}\geq p_{2}\geq\dots\geq p_{m}$
Huffman coding is defined inductively:
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