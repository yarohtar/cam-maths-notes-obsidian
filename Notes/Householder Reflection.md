For $u\neq 0$ we define $H_u=I-2{uu^T\over u^Tu}$. It is symmetric and $H_uH_u=I$, so it is orthogonal.

Suppose $a\neq b$ but $||a||=||b||$. Then by picking $u=a-b$, we find:
$$H_ua=b$$
(just expand and pray)

Now setting $a=(a_1,\dots, a_k,\dots a_n)$ and $b=(a_1,\dots, a_{k-1}, \gamma,0,\dots,0)$ 
we find $u=(0,\dots,0,a_k-\gamma,a_{k+1}\dots,a_n)$ where $\gamma=\sqrt{\sum_{i=k}^na_i^2}$. 
Then $H_u$ doesn't affect the first $k-1$ rows and columns of a matrix, 
and if $a$ is the $k$-th column, we have $H_ua=b$ so we introduced $0$s to the $k$-th column

It is more efficient to calculate $H_uA$ as $A-2{1\over u^Tu}u(u^TA)$ (complexity $O(n^2)$) 
rather than calculating $H_u$ and then multiplying matrices (complexity $O(n^3)$).
