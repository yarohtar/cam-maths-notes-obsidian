Before transmission, parties share some secret information called keys

$$
\mathcal{M}=\{ \text{all possible unencrypted msgs} \}
$$
$$
\mathcal{E}=\{ \text{all possible encrypted msgs} \}
$$
$$
\mathcal{K}=\{ \text{all possible keys} \}
$$
[[Cryptosystem]]
[[Breaking Cryptosystems]]
[[Key Equivocation]]
[[Message Equivocation]]
[[Perfect Secrecy]]
[[Unicity Distance]]
### Lemma 
[[Message Equivocation]]$\leq$[[Key Equivocation]]
$H(M|C)\leq H(K|C)$
#### Proof
Since $M=d(C,K)$, we know $H(M|C,K)=0$
Now calculate:
$$
\begin{align}
H(K|C)&=H(K,C)-H(C) \\
 & =H(M,K,C)-H(M|K,C)-H(C) \\
 & =H(K|M,C)+H(M,C)-H(C) \\
 & =H(K|M,C) +H(M|C)\geq H(M|C)
\end{align}
$$



[[Feedback Shift Register]]
[[Linear Feedback Shift Register]]
[[Berlekamp-Massey algorithm]]
