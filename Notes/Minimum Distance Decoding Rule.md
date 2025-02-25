The minimum distance decoding rule decodes $x\in \{ 0,1 \}^{n}$ as $c\in C$ minimising the [[Hamming distance]] $d(x,c)$.

### Lemma
If the probability of a bit being mismatched is $p<\frac{1}{2}$ then the minimum distance rule agrees with [[Maximum Likelihood Decoding Rule]].

#### Proof
Suppose $d(x,c)=r$
$P(x\text{ recd}| c \text{ sent})=p^{r}(1-p)^{n-r}=(1-p)^{n}\left( \frac{p}{1-p} \right)^{r}$
Since $p<\frac{1}{2}$, choosing $c$ to maximise the above probability is the same as choosing $c$ to minimize $d(x,c)$
