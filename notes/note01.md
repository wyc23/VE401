# Elementary Probability

## Cardano's Principle

Let A be a random outcome of an experiment that may proceed in various ways. Assume each of these way is equally likely,

$$P[A] = \frac{\text{number of ways leading to outcome A}}{\text{number of ways the experiment can proceed}}$$

## Distinguishable or indistinguishable

- Two coins tossed
  - coins are distinguishable
  - {h,t} and {t,h} are different events
  - P[at least 1 head] = $\frac{3}{4}$
  - D'Alembert is wrong
- Bose's inspiration
  - photons are indistinguishable

## Basic principle of counting

- permutation
  - different ways of choosing an ordered tuples of k objects from A
  - $\frac{n!}{(n-k)!}$
- combination
  - different ways of choosing an unordered set of k objects from A
  - $\frac{n!}{k!(n-k)!}$
- permutation of k indistinguishable objects
  - ways of partitioning A into k disjoint subsets
  - $\frac{n!}{n_1!n_2!\ldots n_k!}$

## Binomial coefficients

$\forall \alpha \in \mathbb{R}$
$$\binom{\alpha}{0}:=1$$

and, $\forall n \in \mathbb{N}\backslash \lbrace0\rbrace, \alpha \in \mathbb{R}$
$$\binom{\alpha}{n}:=\frac{\alpha\cdot(\alpha - 1)\cdots(\alpha-n+1)}{n!}$$

## Sample spaces and sample points

- physical outcomes $\rightarrow$ mathematical objects
- mathematical objects: sample points
- sample space: large enough to accommodate all sample points

## Events

- an outcome in the sense of Cardano's principle
- a subspace A of a sample space S
  
Two events $A_1, A_2$ are called mutually exclusive if $A_1 \cap A_2 = \emptyset$

## $\sigma$-Field of subsets

A $\sigma$-Field $\mathscr{F}$ on S is the family of subsets of S such that

1. $\emptyset \in \mathscr{F}$;
2. if $A \in \mathscr{F}$, then $S\backslash A \in \mathscr{F}$;
3. if $A_1,A_2,A_3,\ldots \in \mathscr{F}$ is a finite or countable sequence of subsets, then the union $\bigcup_{k}A_k \in \mathscr{F}$.

- if S is finite, we can take $\mathscr{F}=\mathscr{P}(S)$;
- For any set S, the smallest possible $\sigma$-field is $\mathscr{F}=\lbrace\emptyset,S\rbrace$;
- Borel sets

## Probability measures and spaces

Let S be a sample space and $\mathscr{F}$ a $\sigma$-field on S, the function
$$P:\mathscr{F}\rightarrow[0,1],\hspace{5em}A\to P(A),$$
is called a probability measure (or probability function) on S if

1. $P[S]=1$,
2. for any set of events ${A_k} \subset \mathscr{F}$ such that $A_j \cap A_k = \emptyset$ for $j \neq k$,
   $$P[\bigcup_kA_k]=\sum_kP[A_k]$$.

The triple $(S,\mathscr{F},P)$ is called a probability space.

## Almost sure occurrence

An event $A \in \mathscr{F}$ is said to occur almost surely if $P[A]=1$.
