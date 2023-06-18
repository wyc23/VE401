# Expectation, Variance and Moments

## Expectation

Let $(X,f_X)$ be a discrete random variable, the expected value or expectation of $X$ is
$$E[X]:=\sum_{x\in\Omega}x\cdot f_X(x).$$

We often write $\mu_X$ or simply $\mu$ for the expectation.

## Functions of random variables

Given a random variable $X$, let $Y=\varphi(X)$ and $Y$ is also a random variable with the probability density function
$$f_Y(y)=P[Y=y]=P[\varphi(X)=y]=\sum_{x\in\Omega,\hspace{0.2em}\varphi(x)=y}f_X(x)$$

## Expectation of a function of a random variable

$$E[\varphi\circ X]=\sum_{x\in\Omega}\varphi(x)\cdot f_X(x)$$

## Some properties of expectation

- $E[c]=c$
- $E[cX]=cE[X]$
- $E[X+Y]=E[X]+E[Y]$

## Variance and standard deviation

- variance is the mean square deviation from the mean
- $Var[X]=E[(X-E[X])^2]$
- the standard deviation is defined as $\sigma_X=\sqrt{Var[X]}$

## Some properties of the variance

- $Var[X]=E[X^2]-E[X]^2$
- $Var[c]=0$
- $Var[cX]=c^2Var[X]$

## Standardized random variables

Given a random variable $X$, the standardized random variable is
$$Y=\frac{X-\mu}{\sigma}$$

Notice that $E[Y]=0$ and $Var[X]=1$.

## Ordinary and central moments

- $n^{th}$ (ordinary) moments of $X$: $E[X^n]$,
- $n^{th}$ central moments of $X$: $E[(\frac{X-\mu}{\sigma})^n]$.

## Moment-Generating function

If the power series
$$m_X(t):=\sum_{n=0}^{\infty}\frac{E[X^n]}{n!}t^n$$
has radius of convergence $\varepsilon > 0$,
$$m_X:(-\varepsilon,\varepsilon)\to\mathbb{R}$$
is called the moment-generating function for $X$.

- $$m_X(t)=E[e^{tx}]$$
- $$E[X^k]=\left.\frac{d^km_X(t)}{dt^k}\right|_{t=0}$$