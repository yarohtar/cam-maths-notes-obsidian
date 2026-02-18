# Partition Regular

#ai-generated

Let $A$ be an $m \times n$ matrix with rational entries. We say that $A$ is partition regular (PR) (over $\mathbb{N}$) if whenever $\mathbb{N}$ is finitely coloured, there is always a monochromatic $x \in \mathbb{N}^n$ with $Ax = 0$.

**Examples.** 1. Schur states that the matrix $(1\ 1\ -1)$ is PR.

2. Strengthened Van der Waerden states that the matrix

$$\begin{pmatrix} 1 & 1 & -1 & 0 & \dots & 0 \\ 1 & 2 & 0 & -1 & \dots & 0 \\ \dots & \dots & \dots & \dots & \dots & \dots \\ 1 & m & 0 & 0 & \dots & -1 \end{pmatrix}$$

is PR.

We also talk about 'the equation $Ax = 0$' being PR.

Not every matrix is PR: for example, $(2 - 1)$ is not PR; for we can 2-colour $x \in \mathbb{N}$ by the parity of max$\{i : 2^i | x\}$. Note that $A$ is PR if and only if $\lambda A$ is PR for any $\lambda \in \mathbb{Q} - \{0\}$, so we could restrict our attention to integer matrices if we wished.