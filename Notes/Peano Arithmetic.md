We aim to axiomatize the set of naturals 
The language consists of $\Omega=\{ 0,s,+,\times \}$ and $\Pi=\emptyset$
with arities of $0,s,+,\times$ being $0,1,2,2$ respectively

Peano Arithmetic consists of the following sentences:
$(\forall x)\neg(sx=0)$
$(\forall x)(\forall y)(sx=sy\implies x=y)$
$(\forall x)(x+0=x)$
$(\forall x)(\forall y)(x+sy=s(x+y))$
$(\forall x)(x\times 0=0)$
$(\forall x)(\forall y)(x\times sy=x\times y+x)$
$(\forall y_{1})\dots(\forall y_{n})[(p[0/x]\land(\forall x)(p\implies p[sx /x]))]$