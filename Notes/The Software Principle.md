There is a register machine $U$, called a universal register machine, such that we have the [[Computable Function]]
$$
f_{U,2}(v,u)=\begin{cases}
f_{M,k+1}(\vec{w}) & \text{if } v=code(M) \text{ for register machine }M \\
 & \text{ with upper register index }k \\
 & \text{ and }u=code(C) \text{ for a configuration} \\
 & \text{ with register content }\vec{w}\text{ of length }k+1 \\
\uparrow & \text{otherwise}
\end{cases}
$$
where we use [[Encoding Register Machines]] to prove this.

