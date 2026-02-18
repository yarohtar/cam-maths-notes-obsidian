```markdown
**Hindman's Theorem.** If \(\mathbb{N}\) is finitely coloured then there exist
\(x_1<x_2<\cdots\) in \(\mathbb{N}\) such that the finite-sums set
\(\mathrm{FS}(x_1,x_2,\dots)=\{\sum_{i\in F}x_i:F\subseteq\mathbb{N},\,0<|F|<\infty\}\)
is monochromatic.

**Proof (sketch via ultrafilters).** See [[Ultrafilter]], [[Stone-Čech Compactification]] and [[Idempotent Ultrafilter]] for background.

Write \(\mathbb{N}=A_1\cup\dots\cup A_k\). Choose an idempotent ultrafilter
\(U\in\beta\mathbb{N}\) (existence: [[Idempotent Ultrafilter]]). Since \(U\)
is an ultrafilter some colour-class \(A\) satisfies \(A\in U\).

Idempotence \(U+U=U\) yields
\(\forall_U x\;\forall_U y\; x+y\in A\). By induction on the number of
summands one obtains
\(\forall_U x_1\cdots\forall_U x_m\;\mathrm{FS}(x_1,\dots,x_m)\subseteq A\)
for every finite \(m\).

Inductive construction: for each finite initial segment \(x_1<\dots<x_n\) let
S_n = { t \in \mathbb{N} : \forall_U y\;\mathrm{FS}(x_1,\dots,x_n,t,y)\subseteq A }.
Each \(S_n\) belongs to \(U\) and hence is nonempty (indeed large). Choose
\(x_1\in S_0\), and having chosen \(x_1<\dots<x_n\) pick \(x_{n+1}\in S_n\)
with \(x_{n+1}>x_n\). This is possible because every set in \(U\) meets the
cofinite (and thus infinite) sets one needs to push the sequence strictly
increasing.

By construction every finite sum from \(x_1,x_2,\dots\) lies in \(A\), so
\(\mathrm{FS}(x_1,x_2,\dots)\) is monochromatic. This proves Hindman's
Theorem.
```
If $\mathbb{N}$ is finitely colored, there exist $x_1 < x_2 < \dots$ such that all finite sums $\sum_{i \in F} x_i$ for finite $F \subseteq \{x_1, x_2, \dots\}$ are the same color.

## Proof

The proof relies on the concept of ultrafilters and idempotent ultrafilters in the Stone-Čech compactification of $\mathbb{N}$, denoted $\beta\mathbb{N}$.

### Ultrafilters and $\beta\mathbb{N}$

A filter on $\mathbb{N}$ is a non-empty collection $F \subset P(\mathbb{N})$ such that:
- $\emptyset \notin F$
- If $A \in F$ and $B \supset A$, then $B \in F$
- If $A, B \in F$, then $A \cap B \in F$

An ultrafilter is a maximal filter, i.e., for every $A \subset \mathbb{N}$, either $A \in U$ or $\mathbb{N} \setminus A \in U$.

The set of all ultrafilters on $\mathbb{N}$ is $\beta\mathbb{N}$, which is a compact Hausdorff space. $\mathbb{N}$ embeds into $\beta\mathbb{N}$ via principal ultrafilters.

For an ultrafilter $U$ and a statement $p(x)$, $\forall_U x \, p(x)$ means $\{x : p(x)\} \in U$.

### Idempotent Ultrafilters

An ultrafilter $U$ is idempotent if $U + U = U$, where $U + V = \{A \subset \mathbb{N} : \{x : \{y : x + y \in A\} \in V\} \in U\}$.

The Idempotent Lemma states that in any compact Hausdorff space with an associative left-continuous binary operation, there exists an idempotent element. Thus, there exists an idempotent ultrafilter in $\beta\mathbb{N}$.

### Proof of Hindman's Theorem

Suppose $\mathbb{N} = A_1 \cup A_2 \cup \cdots \cup A_k$ is a finite coloring.

Choose an idempotent ultrafilter $U \in \beta\mathbb{N}$. Since $U$ is an ultrafilter, there exists some $i$ such that $A_i \in U$. Let $A = A_i$.

Since $U$ is idempotent, $\forall_U x \forall_U y \, x + y \in A$.

By induction on finite sums, $\forall_U x \forall_U y \, FS(x, y) \subset A$, where $FS(x, y)$ denotes the set of finite sums from $\{x, y\}$.

Pick $x_1$ such that $\forall_U y \, FS(x_1, y) \subset A$.

Suppose we have $x_1 < x_2 < \cdots < x_n$ such that $\forall_U y \, FS(x_1, \dots, x_n, y) \subset A$.

For each $z \in FS(x_1, \dots, x_n, y)$, we have $\forall_U y \, z + y \in A$, hence $\forall_U x \forall_U y \, z + x + y \in A$.

Thus, $\forall_U x \forall_U y \, FS(x_1, \dots, x_n, x, y) \subset A$.

Pick $x_{n+1} > x_n$ such that $\forall_U y \, FS(x_1, \dots, x_{n+1}, y) \subset A$.

By induction, the sequence $x_1 < x_2 < \cdots$ satisfies that all finite sums from the sequence are in $A$, hence monochromatic.

This completes the proof.