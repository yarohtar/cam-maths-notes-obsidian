Let $A,B,C\subseteq \mathbb{Z}$.
Then 
$$
\lvert A-C \rvert \leq \frac{ \lvert A-B \rvert \lvert B-C \rvert  }{ \lvert B \rvert  }
$$
### Proof
Define functions $a:A-C\to A$ and $c:A-C\to C$ by $a(x)-c(x)=x$
Also define $f:(A-C)\times B\to(A-B)\times(A-C)$ by 
$$
f(x,y) = (a(x)-y, y-c(x))
$$
