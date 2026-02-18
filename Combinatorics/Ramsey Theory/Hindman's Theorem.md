Hindman's Theorem. If \(\mathbb{N}\) is finitely coloured then there exist
\(x_1<x_2<\cdots\) in \(\mathbb{N}\) such that the finite-sums set
\(\mathrm{FS}(x_1,x_2,\dots)=\{\sum_{i\in F}x_i:\emptyset\neq F\subset\mathbb{N},\ |F|<\infty\}\)
is monochromatic.

### Proof

Choose an idempotent ultrafilter \(U\in\beta\mathbb{N}\) (see [[Idempotent Ultrafilter]]).
Given a finite colouring \(\mathbb{N}=A_1\cup\dots\cup A_k\), pick a colour class
\(A\) with \(A\in U\) (see [[Ultrafilter]] and [[Stone-Čech Compactification]] for background and notation).

Idempotence \(U+U=U\) implies
\(\forall_U x\;\forall_U y\; (x+y\in A)\), and a routine induction gives
\(\forall_U x_1\cdots\forall_U x_m\;\mathrm{FS}(x_1,\dots,x_m)\subseteq A\)
for every finite \(m\).

We now choose the sequence inductively. For fixed finite \(x_1,\dots,x_n\), the set
\[S_n=\{t\in\mathbb{N}:\forall_U y\;\mathrm{FS}(x_1,\dots,x_n,t,y)\subseteq A\}\]
is a member of \(U\), hence nonempty; pick \(x_{n+1}\in S_n\) with \(x_{n+1}>x_n\).

By construction every finite sum from \(x_1,x_2,\dots\) lies in \(A\), so
\(\mathrm{FS}(x_1,x_2,\dots)\) is monochromatic. \(\square\)
