# Partition Regular Sets Contain All PR Solutions

#ai-generated

**Corollary 20.** Whenever $\mathbb{N}$ is finitely coloured, some colour class contains solutions to all PR equations.

**Proof.** Suppose not. Then we have $\mathbb{N} = D_1 \cup D_2 \cup \dots \cup D_k$, and, for each $i$, a PR matrix $A_i$ such that $D_i$ does not contain a solution of $A_i x = 0$. Then consider the matrix

$$\begin{pmatrix} A_1 \\ A_2 \\ \vdots \\ A_k \end{pmatrix}$$

This is PR, by the Consistency Theorem, but no $D_i$ contains a solution to it, a contradiction.

We say that $D_i \subset \mathbb{N}$ is partition regular if it contains a solution to every PR equation. So Corollary 20 says that if $\mathbb{N} = D_1 \cup D_2 \cup \dots \cup D_k$ then some $D_i$ is PR. Rado conjectured, and Deuber proved, that if $D$ is PR and $D = D_1 \cup D_2 \cup \dots \cup D_k$ then some $D_i$ is PR.