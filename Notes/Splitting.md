Suppose we use some numerical scheme in the spatial coordinates and get
$$
u'=Au
$$
We might be tempted to say $u=e^{tA}u$.
Unfortunately, computing and controlling the error of $e^{tA}$ is complicated in general, however for some special cases we might get lucky.

Suppose $A=B+C$
Then
$$
e^{ tA }=e^{ tB }e^{ tC }+\frac{1}{2}t^{2}(CB-BC)+O(t^{3})
$$
If $B$ and $C$ commute, then $e^{tA}=e^{B}e^{ C }$

#### Proof
Taylor expand.