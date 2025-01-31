$QR$ factorisation of a $m\times n$ matrix $A$ is $A=QR$ where $Q$ is a $m\times m$ square orthogonal matrix and $R$ is $m\times n$ upper triangular. 
If $m>n$, we can have a reduced $QR$ factorisation with $Q$ being $m\times n$ and $R$ being $n\times n$, where the columns of $Q$ are orthogonal. 

One method for obtaining the $QR$ factorisation is the classic [[Gram-Schmidt process]], where
$$b_j=a_j-\sum_{i=1}^{j-1}{R_{ij}\over ||b_i||}b_i$$
with $q_i={b_i\over ||b_i||}$ and $R_{ij}=<q_i,a_j>$ for $i<j$ and $R_{jj}=||b_j||$.

### Givens rotation
We use the fact that
$$\begin{pmatrix}{\alpha\over\sqrt{\alpha^2+\beta^2}} & \beta\over\sqrt{\alpha^2+\beta^2} \\ -\beta\over\sqrt{\alpha^2+\beta^2} & \alpha\over\sqrt{\alpha^2+\beta^2}\end{pmatrix}\begin{pmatrix}\alpha\\\beta\end{pmatrix}=\begin{pmatrix}\sqrt{\alpha^2+\beta^2}\\ 0\end{pmatrix}$$
To introduce the $0$s from left to right. 

### Householder reflections
For $u\neq 0$ we define $H_u=I-2{uu^T\over u^Tu}$. It is symmetric and $H_uH_u=I$, so it is orthogonal.

Suppose $a\neq b$ but $||a||=||b||$. Then by picking $u=a-b$, we find:
$$H_ua=b$$
(just expand and pray)

Now setting $a=(a_1,\dots, a_k,\dots a_n)$ and $b=(a_1,\dots, a_{k-1}, \gamma,0,\dots,0)$ we find $u=(0,\dots,0,a_k-\gamma,a_{k+1}\dots,a_n)$ where $\gamma=\sqrt{\sum_{i=k}^na_i^2}$. Then $H_u$ doesn't affect the first $k-1$ rows and columns of a matrix, and if $a$ is the $k$-th column, we have $H_ua=b$ so we introduced $0$s to the $k$-th column. 
It is more efficient to calculate $H_uA$ as $A-2{1\over u^Tu}u(u^TA)$ (complexity $O(n^2)$) rather than calculating $H_u$ and then multiplying matrices (complexity $O(n^3)$).
