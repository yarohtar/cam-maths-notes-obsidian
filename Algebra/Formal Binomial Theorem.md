In any [[Algebra/Ring Theory/Ring|Ring]] $R$, we can write
$$
(1+x)^{r} = \sum_{n\geq 0} \binom{ r }{ n } x^{n}
$$
as a [[Formal Power Series]], where 
$$
\binom{ r }{ n } = \frac{ r ^{\underline{ n }} }{ n! }
$$
### Proof
Let $f(x)=(1+x)^{r}=\exp(r\log(1+x))$
Then
$$
f'(x) = \frac{ r }{ 1+x } f(x) = r\exp(-\log(1+x)) \exp(r\log(1+x))
$$
and thus 
$$
f'(x) = r(1+x)^{r-1}
$$
Then calculate 
$$
f^{(n)}(x) = r^{\underline{ n }} (1+x)^{r-n}
$$
so 
$$
f^{(n)}(0) = r^{\underline{ n }}
$$

