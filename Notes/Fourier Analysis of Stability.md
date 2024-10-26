Assume a recurrence of the form:
$$
\sum_{k}a_{k}u_{m+k}^{n+1}=\sum_{k}b_{k}u_{m+k}^{n}
$$
## Amplification factor
Let $\hat{u}^n=\sum_{m}e^{-im\theta}u_{m}^n$ for all $n$ (by using [[Fourier Transform#Sequences]])
Multiply both sides by $e^{-im\theta}$ and sum both sides over $m\in \mathbb{Z}$:
$$
\begin{align}
LHS & =\sum_{m}e^{-im\theta}\sum_{k=r}^{s} a_{k}u_{m+k}^{n+1} \\
 & = \sum_{k=r}^{s}a_{k}\sum_{m}e^{-im\theta}u_{m+k}^{n+1}\\
 & =\sum_{k=r}^{s}a_{k}\sum_{m}e^{-i(m-k)\theta}u_{m}^{n+1} \\
 & \left( \sum_{k=r}^{s}a_{k}e^{ik\theta} \right)\hat{u} ^{n+1}(\theta) \\
 \\
RHS & =\left( \sum_{k=r}^{s}b_{k}e^{ik\theta} \right)\hat{u}^{n+1}(\theta)
\end{align}
$$
Hence we find:
$$
\hat{u}^{n+1}(\theta)=H(\theta)\hat{u}^{n}(\theta)
$$
with
$$
H(\theta)= \frac{\sum_{k=r}^{s}b_{k}e^{ik\theta}}{\sum_{k=r}^{s} a_{k}e^{ik\theta}}
$$
### Theorem
The method is stable iff $\lvert H(\theta) \rvert\leq 1$ for all $\theta \in[-\pi,\pi]$.
#### Proof
One side is easy, due to the above calculations and [[Parseval's Identity]].

