## Postulate I
States are vectors $\ket{\psi}$ in a [[Hilbert Spaces (PQM)|Hilbert space]] $\mathcal{H}$.
## Postulate II
[[Observables]] are [[Linear Operators|linear]] [[Adjoint|Hermetian]] operators $Q:\mathcal{H}\to \mathcal{H}$.

tikz \usepackage{tikz-cd} \begin{document} \begin{tikzcd}     T     \arrow[drr, bend left, "x"]     \arrow[ddr, bend right, "y"]     \arrow[dr, dotted, "{(x,y)}" description] & & \\     K & X \times_Z Y \arrow[r, "p"] \arrow[d, "q"]     & X \arrow[d, "f"] \\     & Y \arrow[r, "g"]     & Z \end{tikzcd} \quad \quad \begin{tikzcd}[row sep=2.5em] A' \arrow[rr,"f'"] \arrow[dr,swap,"a"] \arrow[dd,swap,"g'"] &&   B' \arrow[dd,swap,"h'" near start] \arrow[dr,"b"] \\ & A \arrow[rr,crossing over,"f" near start] &&   B \arrow[dd,"h"] \\ C' \arrow[rr,"k'" near end] \arrow[dr,swap,"c"] && D' \arrow[dr,swap,"d"] \\ & C \arrow[rr,"k"] \arrow[uu,<-,crossing over,"g" near end]&& D \end{tikzcd} \end{document}
