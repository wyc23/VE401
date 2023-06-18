# Conditional Probability

## Conditional probability

We denote
$$P[B|A]:=\frac{P[A\cap B]}{P[A]},\hspace{3em}P[A]\neq 0$$
the conditional probability that "B occurs given A has occurred"

## Independence of events

We say two events A and B are independent if
$$P[A\cap B]=P[A]P[B],$$

this is equivalent to
$$P[A|B]=P[A]\hspace{5em}\text{if }P[B]\neq 0,\\
P[B|A]=P[B]\hspace{5em}\text{if }P[A]\neq 0.$$

## Total probability

We take a set of n, pairwise mutually exclusive events $A_1,A_2,\ldots,A_n$ in the sample space S such that $P[A_k]\neq 0$ and $A_1\cup\ldots A_n=S$, then for any event $B \subset S$,
$$P[B]=\sum_{k=1}^n P[B|A_k]\cdot P[A_k],$$
is called the total probability formula for $P[B]$.

## Bayes's theorem

Let $A_k$ be be the same as before, $P[B] \neq 0$,
$$P[A_k|B]=\frac{P[B\cap A_k]}{P[B]}=\frac{P[B|A_k]\cdot P[A_k]}{\sum_{j=1}^nP[B|A_j]\cdot P[A_j]}$$
