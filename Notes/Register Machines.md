Register machines can perform the following $Q$-instructions:

| Instruction            | Interpretation                                                                                                                             |
| ---------------------- | ------------------------------------------------------------------------------------------------------------------------------------------ |
| $+_{a}(k,q)$           | Add letter $a$ to the content of register $k$ and go to state $q$                                                                          |
| $?_{a}(k,q,q')$        | Check whether the last letter in register $k$ is $a$<br>- If so go to state $q$<br>- otherwise go to state $q'$                            |
| $?_{\epsilon}(k,q,q')$ | Same as before just with empty register                                                                                                    |
| $-(k,q,q')$            | Check whether register $k$ is empty<br>- If so go to state $q$<br>- Otherwise, remove the final letter of its content and go to state $q'$ |

### Definition
A pair $M=(Q,P)$ is called a register machine if $Q$ is a non-empty finite set of states with two special elements $q_{S}\neq q_{H}$ (start and halt states), and $P$ is a function with domain $Q$ and codomain the $Q$-instructions (so each $P(q)$ is a $Q$-instruction). 
The function $P$ is called the program of the register machine.
For a fixed $q\in$