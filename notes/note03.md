# Discrete Random Variables

## Random variable

The function that take elements of a sample space and map them into a subset of the real numbers:
$$X:S\to\mathbb{R},$$
such a function X is said to be a random variable.

## Discrete random variables

Let S be a sample space and $\Omega$ a countable subset of $\mathbb{R}$. A discrete random variable is a map
$$X:S\to\Omega$$
together with a function
$$f_X:\Omega\to\mathbb{R}$$
having the properties that

1. $f_X(x)\ge 0$ for all $x \in \Omega$,
2. $\sum_{x\in\Omega}f_X(x)=1$.

The function $f_X$ is called the probability density function or probability distribution of X.

A random variable id given by pair $(X,f_X)$,$f_X(x)=P[X=x]$.

## Bernoulli random variable

- a signal trial with the success probability $p\in(0,1)$
- $$X:S\to\lbrace0,1\rbrace$$
- $$f_X:\lbrace0,1\rbrace\to\mathbb{R},\hspace{3em}
    f_X(x)=
    \begin{cases}
        1-p & \text{if} & x=0\\
        p & \text{if} & x=1
    \end{cases}$$
- $$X \sim \text{Bernoulli}(p)$$

## Binomial random variable

- the number of success in $n$ independent and identical Bernoulli trials
- $$X:S\to\Omega=\lbrace0,\ldots,n\rbrace$$
- $$f_X:\Omega\to\mathbb{R},\hspace{3em}f_X(x)=\binom{n}{x}p^x(1-p)^{n-x}$$
- $$X \sim \text{B}(n,p)$$

## Cumulative distribution function

The cumulative distribution function of a random variable is defined as:
$$F_X:\mathbb{R}\to\mathbb{R},\hspace{3em}F_X(x):=P[X\le x],$$
for a discrete random variable,
$$F_X(x)=\sum_{y\le x}f_X(y).$$

## Geometric distribution

- the number of trials needed to obtain the first success in a sequence of Bernoulli trials
- $$X:S\to\Omega=\mathbb{N}\backslash\lbrace0\rbrace$$
- $$f_X(x)=(1-p)^{x-1}p$$
- $$X \sim \text{Geom}(p)$$
