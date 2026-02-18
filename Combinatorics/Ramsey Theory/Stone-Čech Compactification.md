The Stone-Čech compactification $\beta X$ of a [[Topological Space]] $X$ is the largest [[Compact]] [[Hausdorff]] space in which $X$ is densely embedded.

For $X = \mathbb{N}$, $\beta \mathbb{N}$ can be identified with the set of [[Ultrafilter]]s on $\mathbb{N}$, with the topology where basic open sets are $\{ u : A \in u \}$ for $A \subseteq \mathbb{N}$.

## Theorem

$\beta \mathbb{N}$ is [[Compact]] [[Hausdorff]].

## Proof

Hausdorff: Given distinct ultrafilters $u, v$, there is $A \in u \setminus v$, so $A^c \in v$, and $C_A \cap C_{A^c} = \varnothing$.

Compact: Use the fact that ultrafilters are closed under finite intersections, and apply Alexander's subbase theorem or similar.

#ai-generated