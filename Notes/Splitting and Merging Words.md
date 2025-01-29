Consider:
$$
z:(i,j)\to \frac{(i+j)(i+j+1)}{2}+j
$$
which is the Cantor zigzag function. 
This function is in the class of [[Gödel's primitive recursive functions]] so it is [[Computable Function]]. 

So the map $(v,w)\to u$ if $\#u=z(\#v,\#w)$ is a computable function.
We write $v*w=u$ and call this operation merging.

The inverse of this operation is also [[Computable Function]] and we call this splitting:
$$
\cdot_{(0)}:\mathbb{B}\to \mathbb{B}
$$
$$
\cdot_{(1)}:\mathbb{B}\to \mathbb{B}
$$
such that 
$$
u_{(0)}*u_{(1)}=u
$$
