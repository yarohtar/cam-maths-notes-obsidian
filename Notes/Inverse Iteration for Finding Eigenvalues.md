Given some $s$, we set:
$$
(A-sI) x^{k+1}=x^{k}
$$
This converges to an eigenvector with eigenvalue closest to $s$
We can make it faster by adjusting $s$ throughout the iteration
Take $s ^{k+1}$ to be the minimizer of $f(s)=\lVert Ax^{k+1} - s ^{k+1} x^{k+1} \rVert$
