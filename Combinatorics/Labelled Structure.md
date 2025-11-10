### Definition
Given labelled structures $\mathcal{A}=(A,v_{A})$ and $\mathcal{B}=(B,v_{B})$ define the following:

| Operation         | Symbol                         | Objects of size $n$                                                                                                                                   | Valuation                             |
| ----------------- | ------------------------------ | ----------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------- |
| Disjoint Union    | $\mathcal{A}+\mathcal{B}$      | $(A\sqcup B)_{n}$                                                                                                                                     | $v_{A}\cup v_{B}$                     |
| Labelled Product  | $\mathcal{A}*\mathcal{B}$      | $\bigcup_{S\cup T=[n]}\{ (\alpha \vert _{S},\beta \vert _{T}):\alpha \in A,\beta \in B \}$                                                            | $v_{A}(\alpha)\cdot v_{B}(\beta)$     |
| Labelled Sequence | $\mathrm{Seq}(\mathcal{A})$    | $\bigcup_{k\geq 0}\bigcup_{S_{1}\cup \dots \cup S_{k}=[n]}\{ (\alpha_{1}\vert_{S_{1}},\dots,\alpha_{k}\vert_{S_{k}}) : \alpha_{i} \in \mathcal{A} \}$ | $\prod_{i=1}^{k}v_{A}(\alpha_{i})$    |
| Labelled Set      | $\mathrm{Set}(\mathcal{A})$    | $\bigcup_{k\geq 0}\bigcup_{S_{1}\cup\dots \cup S_{k}=[n]}\{ \{ \alpha_{1}\vert_{S_{1}},\dots ,\alpha_{k}\vert_{S_{k}} \}:\alpha_{i}\in A \}$          | $\prod_{i=1}^{k}v_{A}(\alpha_{i})$    |
| Composition       | $\mathcal{B}\circ \mathcal{A}$ | $\bigcup_{k\geq 0}\bigcup_{S_{1}\cup\dots \cup S_{k}=[n]}\{ (\beta,\{ \alpha_{1}\vert_{S_{1}},\dots,\alpha_{k}\vert_{S_{k}} \}):\alpha_{i}\in A \}$   | $w_{B}(\beta)\prod v_{A}(\alpha_{i})$ |
| Shifted           | $\mathcal{A}_{+}$              | $\{ \alpha \in A_{n+1} \text{ built on }[n]\cup[t] \}$                                                                                                | $v_{A}(\alpha)$                       |
| Root              | $\mathcal{A}_{\bullet}$        | $\{ (\alpha,r) : \alpha \in A_{n} \text{ built on }[n]; r\in[n] \}$                                                                                   | $v_{A}(\alpha)$                       |

[[Dictionary of Operations]]
[[Combinatorial Union]]
[[Combinatorial Product]]
