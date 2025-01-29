We can represent a [[Register Machine]] $M=(Q,P)$ as a list of instructions, where the $i$-th instruction in the list represents $P(q_{i})$. 
Being careful about stuff, we can encode it into some encoding alphabet. Call $\mathbb{W}$ to denote the words in this alphabet and write $code(M)\in \mathbb{W}$ for this encoding.
Then we can use [[Encoding Alphabets in Binary Words]] to encode the register machine into binary. 
We can do a similar thing with [[Configuration of a Register Machine]] $C$

Let these encodings be $code(M)$ and $code(C)$ 