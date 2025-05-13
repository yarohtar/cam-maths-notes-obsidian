A nontrivial [[Index Set]] cannot be computable.
### Proof
For a fixed $w$ consider the following function
$$
g_{w}(u,v)=\begin{cases}
f_{w,1}(v) & \text{if } u\in K \\
\uparrow & \text{otherwise}
\end{cases}
$$
Note that $g_{w}$ is computable, as we can run $f_{u,1}(u)$ and if $u\not\in K$ then it will diverge. Otherwise, we run $f_{w,1}(v)$.

By [[The s-m-n Theorem]] we get a computable function $h_{w}$ such that 
$$
f_{h_{w}(u),1}(v) = g_{w}(u,v)
$$
If $u\in K$ then $W_{h_{w}(u)}=W_{w}$. 