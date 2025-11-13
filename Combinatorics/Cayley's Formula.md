Let $R$ be a [[Algebra/Ring Theory/Ring|Ring]] and let $x_{1},x_{2},\dots,x_{n}\in R$.
Consider a tree on nodes $1,2,\dots,n$ 
with edges directed away from some root
and with weights defined by 
$$
w(ij) = x_{i}
$$
Define the weight of the tree $T$ as: 
$$
w(T) = \prod_{e\in T} w(e)
$$
Then the sum of weights of all possible such trees is:
$$
p_{n}(x_{1},x_{2},\dots,x_{n}) = (x_{1}+x_{2}+\dots+x_{n})^{n-1}
$$
### Proof
Note that $p_{n}$ is a symmetric, homogeneous polynomial of degree $n-1$.
The weight of trees with leaf node $n$ is $p_{n}(x_{1},\dots,x_{n-1},0)$
Counting another way, we find 
$$
p_{n}(x_{1},\dots,x_{n-1},0) = (x_{1}+\dots+x_{n-1}) p_{n-1}(x_{1},\dots,x_{n-1})
$$
Proceed by induction. 
For $n=2$ we can check $p_{2}(x_{1},x_{2})=x_{1}+x_{2}$ (there are only 2 trees).
Now assume that 
$$
p_{n-1}(x_{1},\dots,x_{n-1})=(x_{1}+\dots+x_{n-1})^{n-2}
$$
We conclude that 
$$
p_{n}(x_{1},\dots,x_{n-1},0) = (x_{1}+\dots+x_{n-1})^{n-1}
$$
Consider $r_{n}(x_{n})=p_{n}(x_{1},\dots,x_{n})-(x_{1}+\dots+x_{n})^{n-1}$.
This is a symmetric, homogeneous polynomial of degree $n-1$.
Also 