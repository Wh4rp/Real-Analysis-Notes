# Metric Space
:::{prf:definition} Metric Space
:label: metric-space

Let be $X$ a set nonempty. A function $\rho : X \times X \to \mathbb{R}$ is a _distance function_ if and only if $\forall x, y, z \in X$ such that:
1. $f(x, y) \geq 0$
2. $f(x, y) = 0 \Leftrightarrow x = y$
3. $f(x, y) = f(y, x)$
4. $f(x, y) \leq f(x, z) + f(z, y)$

In that case a $(X, \rho)$ we called ***metric space***.
:::

:::{prf:example}
$X = \mathbb{R}$

$x = (x_1, x_2)$, $y = (y_1, y_2)$

$d(x, y) = \sqrt{(x_1 - y_1)^2 + (x_2 - y_2)^2}$

$(\mathbb{R}, d)$ is a *m.e.*
:::

:::{prf:example}
$X = \mathbb{R}$

$x = (x_1, x_2)$, $y = (y_1, y_2)$

$d_{\infty}(x, y) = \max \{|x_1 - y_1|, |x_2 - y_2| \}$

$(\mathbb{R}, d_{\infty})$ is a *m.e.*
:::

:::{prf:example}
$X = \{ f:[0,1] \to \mathbb{R}\ | \ f \text{ is continuous}\}$

$x = (x_1, x_2)$, $y = (y_1, y_2)$

$\rho(f, g) = \int_0^1 |f(x) - g(x)| dx$

$\sigma(f, g) = \max \{ |f(x) - g(x)|, \ x \in [0, 1] \}$
:::

## Varous definitions

:::{prf:definition} Neighbourhood
:label: neighbourhood

Let be $X$ a metric space and $p \in X$. A neighborhood of $p$ is a set $N_r(p)$ consisting of all $q$ such that $d(p, q) < r$, for some $r > 0$. The number $r$ is called the _radius_ of $N_r(p)$. 
:::

:::{prf:definition} Limit Point
:label: limit-point

Let be $X$ a metric space and $p \in X$. A point $p$ is a _limit point_ of the set $E \subset X$ if every neighborhood of $p$ constain a point $q \neq p$ such that $q \in E$.
:::

:::{prf:definition} Isolated Point
:label: isolated-point

Let be $X$ a metric space, $p \in X$ and $E \subset X$. If $p \in E$ and $p$ is not limit point of $E$, then $p$ is called an _isolated point_. 
:::

:::{prf:definition} Closed
:label: closed

Let be $X$ a metric space and $E \subset X$. $E$ is _closed_ if every limit point of $E$ is a point of $E$. 
:::

:::{prf:definition} Interior (point)
:label: interior-point

Let be $X$ a metric space, $p \in X$ and $E \subset X$. A point $p$ is an _interior point_ of $E$ if there is a neighborhood $N$ of $p$ such that $N \subset E$.
::: 

:::{prf:definition} Open
:label: open

Let be $X$ a metric space and $E \subset X$. $E$ is _open_ if every point of $E$ is an interior point of $E$. 
:::

:::{prf:definition} Bounded
:label: bounded

Let be $X$ a metric space, $p, q \in X$ and $E \subset X$. $E$ is _bounded_ if there is a real number $M$ and a point $p \in X$ such that $d(p, q) < M$ for all $p \in E$. 
:::

:::{prf:definition} Dense
:label: dense

Let be $X$ a metric space and $E \subset X$. $E$ is _dense_ in $X$ if every point of $X$ is limit point of $E$, or a point of $E$ (or both). 
:::

::::{prf:theorem}

Every neighborhood is an open set.

:::{admonition} Proof
:class: dropdown

Consider a neighborhood $E=N_{p}(p)$, and let $q$ be any point of $E$. Then there is a positive real number $h$ such that

$$
d(p, q)=r-h .
$$

For all points $s$ such that $d(q, s)<h$, we have then

$$
d(p, s) \leq d(p, q)+d(q, s)<r-h+h=r,
$$

so that $s \in E$. Thus $q$ is an interior point of $E$.
:::

::::


