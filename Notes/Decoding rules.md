The error rate depends on the decoding rule. We consider 3 possible rules:
1. [[Ideal Observer Decoding Rule]]
2. [[Maximum Likelihood Decoding Rule]]
3. [[Minimum Distance Decoding Rule]]
#### Remark
Some convention needed in the case of a tie, eg. choose at random or ask for message to be sent again.

[[Hamming distance]]


### Lemma
If $p<\frac{1}{2}$ then 2. and 3. agree
#### Proof
Suppose $d(x,c)=r$
$P(x\text{ recd}| c \text{ sent})=p^{r}(1-p)^{n-r}=(1-p)^{n}\left( \frac{p}{1-p} \right)^{r}$
Since $p<\frac{1}{2}$, choosing $c$ to maximise the above probability is the same as choosing $c$ to minimize $d(x,c)$


