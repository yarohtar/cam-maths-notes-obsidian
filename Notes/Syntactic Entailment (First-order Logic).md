## Axioms
1. $p\implies(q\implies p)$
2. $(p\implies(q\implies r))\implies((p\implies q)\implies(p\implies r))$
3. $\neg \neg p\implies p$
4. $(\forall x)(x=x)$
5. $(\forall x)(\forall y)((x=y)\implies(p\implies p[y/ x]))$
(where $p$ is any formula with no bound occurrence of $y$)
6. $(\forall x)p\implies p[t/ x]$
($p$ is a formula with $x\in FV(p)$ and $t$ is a term no variable of which occurs bound in $p$)
1. $(\forall x)(p\implies q)\implies(p\implies(\forall x)q)$