$$
H(X|Y=y)=-\sum_{x\in \Sigma_{1}}P(X=x|Y=y)\log P(X=x|Y=y)
$$
$$
H(X|Y)=\sum_{y\in \Sigma_{2}}P(Y=y)H(X|Y=y)
$$
### Lemma
$H(X,Y)=H(X|Y)+H(Y)$
#### Proof
$$
H(X|Y)=-\sum_{y\in \Sigma_{2}}\sum_{x\in \Sigma_{1}}P(X=x|Y=y)P(Y=y)\log P(X=x|Y=y)
$$