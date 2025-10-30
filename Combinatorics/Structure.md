A structure $\mathcal{A}=(A,v)$ is a countable set $A$ of combinatorial objects
equipped with a valuation $v:A\to R[x]$ such that 
$$
v(\alpha) = w(\alpha)x^{n}
$$
where $n$ is called the size of $\alpha$ 
and $w(\alpha)\in R$ is called the weight (often $w(\alpha)=1$ for all $\alpha$)
and moreover 
$$
A_{n} = \{ \alpha \in A \text{ of size }n \}
$$
is finite for all $n$, so the [[Generating Function]]
$$
f_{\mathcal{A}}(x) = \sum_{\alpha \in A} v(\alpha) \in R[[x]]
$$
is well defined,
as is the exponential gen fn 
$$
\tilde{f}_{\mathcal{A}} (x) = \sum_{n\geq 0} \sum_{\alpha \in A_{n}} \frac{ v(\alpha) }{ n! }
$$
