Register machines can perform the following instructions:

| Instruction     | Interpretation                                                                                                  |
| --------------- | --------------------------------------------------------------------------------------------------------------- |
| $+_{a}(k,q)$    | Add letter $a$ to the content of register $k$ and go to state $q$                                               |
| $?_{a}(k,q,q')$ | Check whether the last letter in register $k$ is $a$<br>- If so go to state $q$<br>- otherwise go to state $q'$ |
|                 |                                                                                                                 |
