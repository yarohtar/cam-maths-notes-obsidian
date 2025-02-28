Let $C$ be a $(n,k)$ [[Linear Code]]
A parity check matrix is a [[Generator Matrix]] for $C^{\bot}$
It is a $(n-k)\times n$ matrix 

### Lemma
An $(n,k)$ [[Linear Code]] with [[Generator Matrix]] $G=(I_{k}|B)$ has parity check matrix $H=(-B^{T}|I_{n-k})$
### Proof
Since $GH^{T}=(I_{k}|B)\begin{pmatrix}-B\\I_{n-k}\end{pmatrix}=-B+B=0$
So rows of $H$ generate a subcode of $C^{\bot}$
But $dim(C^{\bot})=n-k=rk(smth)$
Thus the rows of $H$ are a basis for $C^{\bot}$ as required.
