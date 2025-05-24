The integrals
$$
C(x) = \int_{-\infty}^{\infty} \cos(xt^{2}) dt
$$
$$
S(x) = \int_{-\infty}^{\infty} \sin(xt^{2})dt
$$
are called Fresnel integrals.
Using the substitution $s=xt^{2}$ we find
$$
C(x) = \frac{2}{\sqrt{ x }} \int_{0}^{\infty} \frac{\cos s}{\sqrt{ s }} ds
$$
and similar for $S$ and we find:
$$
C(x) = \frac{C(1)}{\sqrt{ x }}
$$
$$
S(x) = \frac{S(1)}{\sqrt{ x }}
$$
Now to evaluate $C(1)$ we note:
$$
\frac{1}{\sqrt{ s }} = \frac{1}{\sqrt{ \pi }} \int_{-\infty}^{\infty} e^{-s\lambda^{2}} d\lambda
$$
Now sub that into the above expression, 
change order of integration
and do some integration by parts
Should get 
$$
C(1) = \sqrt{ \frac{\pi}{2} }
$$
Similarly, $S(1)=C(1)$
By adding and subtracting these integrals we get:
$$
\int_{-\infty}^{\infty} e^{\pm ixt^{2}}dt =C(x) + iS(x) = (1\pm i) \sqrt{ \frac{\pi}{2x} }
$$

