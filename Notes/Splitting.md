Suppose $A=B+C$
Then
$$
e^{ tA }=e^{ tB }e^{ tC }+\frac{1}{2}t^{2}(CB-BC)+O(t^{3})
$$
If $B$ and $C$ commute, then $e^{tA}=e^{tB}e^{ tC }$
#### Proof
Taylor expand.

### Splitting
Now suppose we are solving the diffusion equation 
$$
u_{t}=u_{x x} u_{y y}
$$

This allows for writing:
$$
u^{n+1}=e^{tB}e^{tC}u^{n}
$$
where we can now use
$$
r(z)=\left( 1+\frac{z}{2} \right)\left( 1-\frac{z}{2} \right)^{-1}
$$
to approximate the exponential.

In particular in the case of [[Numerical Methods for Diffusion Equation]]
