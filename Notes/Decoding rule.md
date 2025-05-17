After receiving a [[Binary Code]] through a [[Binary Symmetric Channel (BSC)]], we need to decode it.

There are 3 rules we consider when decoding:
#### Ideal Observer
The ideal observer decoding rule decodes $x\in \{ 0,1 \}^{n}$ as the codeword $c\in C$ maximising $P(c \text{ sent} | x \text{ received})$

This is actually the most reasonable decoding rule but it assumes that the observer has information about the probability of each message being sent.

#### Maximum likelihood
The maximum likelihood decoding rule decodes $x\in \{ 0,1 \}^{n}$ as $c\in C$ maximising $P(x \text{ received}|c \text{ sent})$

### Lemma
If all messages are equally likely then maximum likelihood agrees with the [[Ideal Observer Decoding Rule]].
#### Proof
By Baye's rule trivial.



We send a [[Binary Code]] through a [[Binary Symmetric Channel (BSC)]] making $n$ uses of the channel. Probability $p$ is the probability of a bit being mismatched.

The error rate depends on the decoding rule. We consider 3 possible rules:
1. [[Ideal Observer Decoding Rule]]
2. [[Maximum Likelihood Decoding Rule]]
3. [[Minimum Distance Decoding Rule]] (we use this one)
#### Remark
Some convention needed in the case of a tie, eg. choose at random or ask for message to be sent again.

