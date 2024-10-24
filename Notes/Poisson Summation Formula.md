$$\sum_nf(x+n)=\sum_n\hat f(2\pi n)e^{2\pi i n x}$$
Derivation: note that both sides are 1-periodic so just calculate the Fourier series. Note that RHS immediately gives coefs $\hat f(2\pi n)$ while LHS will conveniently become a Fourier transform. 
($\sum_n\int_0^1$ goes to $\sum_n\int_n^{n+1}=\int_{-\infty}^\infty$ after substitution $y=x+n$)