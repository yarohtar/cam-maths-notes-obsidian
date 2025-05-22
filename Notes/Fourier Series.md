For an $L$-periodic function $f$, we write:
$$f(x)\sim \sum_n \hat{f}_ne^{2\pi inx\over L}$$
where $\hat{f}_n=\frac 1 L \langle f,e^{2\pi inx/L} \rangle$. 
Note that we are summing over $n\in\mathbb Z$.

Call $e_n(x)=e^{2\pi inx\over L}$. 
Then $\langle e_{n},e_{m} \rangle=L\delta_{nm}$.
This is known as the complex Fourier series of $f$.
[[Parseval's Identity]] for $L$-periodic functions $f$ and $g$ is:
$$
\langle f,g\rangle = L\sum_nf_n\overline{g_n}
$$
By writing $a_n=f_n+f_{-n}$ and $b_n=i(f_n-f_{-n})$, 
we find the Fourier series of $f$:
$$f(x)\sim \frac 1 2 a_0 + \sum_{n=1}^\infty a_n\cos{2\pi i n x\over L} + \sum_{n=1}^\infty b_n \sin{2\pi i nx\over L}$$
where $a_n=\frac 2 L \left\langle  f, \cos \frac{2\pi nx}{L}  \right\rangle$ and $b_n=\frac 2 L \langle f,\ \sin{2\pi n x\over L}\rangle$.

Call these $c_n=\cos$, $s_n=\sin$, then:
$\langle c_n,c_m\rangle =\frac L 2 \delta_{nm}$
$\langle s_n, s_m\rangle =\frac L 2 \delta_{nm}$
$\langle 1,c_n\rangle = \langle 1,s_m\rangle = \langle c_n, s_m\rangle = 0$

### Convergence of Fourier series
Define:
$$S_Nf=\sum_{|n|\leq N}f_n e_n$$
Then if $f$ is continuous on $[0,L)$ 
apart from finitely many jump discontinuities 
and $f$ has a finite number of minima and maxima on $L$ 
we have for all $x$:
$${f(x_-)+f(x_+)\over 2} = \lim_{N\to\infty}(S_Nf)(x)$$
### Sine and cosine series
For a function $f:[0,L)\to \mathbb C$ 
we can define it's even and odd extensions $f_{even}$ and $f_{odd}$. 
These are then $2L$ periodic functions
We can find their Fourier series in terms of cosines and sines respectively. 
Hence we found a sine series for $f$ and a cosine series for $f$.
