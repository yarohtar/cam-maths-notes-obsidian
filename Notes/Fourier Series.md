For a $L$-periodic function $f$, we write:
$$f(x)\sim \sum_n f_ne^{2\pi inx\over L}$$
where $f_n=\frac 1 L <f,\ e^{2\pi i nx\over L}>$. Note that we are summing over $n\in\mathbb Z$.

Call $e_n(x)=e^{2\pi inx\over L}$. Then $<e_n,\ e_m>=L\delta_{nm}$.

This is known as the complex Fourier series of $f$.

By writing $a_n=f_n+f_{-n}$ and $b_n=i(f_n-f_{-n})$, we find the Fourier series of $f$:
$$f(x)\sim \frac 1 2 a_0 + \sum_{n=1}^\infty a_n\cos{2\pi i n x\over L} + \sum_{n=1}^\infty b_n \sin{2\pi i nx\over L}$$
where $a_n=\frac 2 L<f,\ \cos{2\pi nx\over L}>$ and $b_n=\frac 2 L <f,\ \sin{2\pi n x\over L}>$.

Call these $c_n=\cos$, $s_n=\sin$, then:
$<c_n,c_m> =\frac L 2 \delta_{nm}$
$<s_n, s_m> =\frac L 2 \delta_{nm}$
$<1,c_n> = <1,s_m> = <c_n, s_m> = 0$

### Convergence of Fourier series
Define:
$$S_Nf=\sum_{|n|\leq N}f_n e_n$$
Then if $f$ is continuous on $[0,L)$ apart from finitely many jump discontinuities and $f$ has a finite number of minima and maxima on $L$ we have for all $x$:
$${f(x_-)+f(x_+)\over 2} = \lim_{N\to\infty}(S_Nf)(x)$$
### Sine and cosine series
For a function $f:[0,L)\to \mathbb C$ we can define it's even and odd extensions $f_{even}$ and $f_{odd}$. These are then $2L$ periodic functions and we can find their Fourier series in terms of cosines and sines respectively. Hence we found a sine series for $f$ and a cosine series for $f$.

### Parseval's theorem
$$<f,g> = L\sum_nf_n\overline{g_n}$$
