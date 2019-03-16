# 1 The Real and Complex Number Systems


## Ordered Sets


### 1.6 Definition
An **ordered set** is a set $S$ in which an order is defined.

### 1.7 Definition
Suppose $S$ is an ordered set, and $E \subset S$. If there exists a $\beta \in S$ such that $x \le \beta$ for every $x \in E$, we say that $E$ is **bounded above**, and call $\beta$ an **upper bound** of $E$.

Lower bounds are defined in the same way (with $\ge$ in place of $\le$).

### 1.8 Definition
Suppose $S$ is an ordered set, $E \subset S$, and $E$ is bounded above. Suppose there exists an $\alpha \in S$ with the following properties:
1. $\alpha$ is an upper bound of E.
2. If $\gamma < \alpha$ then $\gamma$ is not an upper bound of $E$.

Then $\alpha$ is called the **least upper bound** of $E$ or the **supremum** of $E$, and we write

$\alpha = \sup E$.

The **greatest lower bound**, or **infimum**, of a set $E$ which is bounded below is defined in the same manner: The statement

$\alpha = \inf E$.

means that $\alpha$ is a lower bound of $E$ and that no $\beta$ with $\beta > \alpha$ is a lower bound of $E$.



# 2 Basic Topology


## Finite, Countable, and Uncountable Sets


### 2.1 Definition
Consider two set $A$ and $B$, whose elements may be any objects whatsoever, and suppose that with each element $x$ of $A$ there is associated, in some manner, an elment of $B$, which we denote by $f(x)$. Then $f$ is said to be a **function** from $A$ to $B$ (or a **mapping** of A into B). The set $A$ is called the **domain** of $f$ (we also say $f$ is defined on $A$), and the elements $f(x)$ are called the **values** of $f$. The set of all values of $f$ is called the **range** of $f$.

### 2.2 Definition
Let $A$ and $B$ be two sets and let $f$ be a mapping of $A$ into $B$. If $E \subset A$, $f(E)$ is defined to be the set of all elements $f(x)$, for $x \in E$. We call $f(E)$ the **image** of $E$ under $f$. In this notation, $f(A)$ is the range of $f$. It is clear that $f(A) \subset B$. If $f(A) = B$, we say that $f$ maps $A$ **onto** $B$. (Note that, according to this usage, **onto** is more specific than **into**.)

If $E \subset B$, $f^{-1}(E)$ denotes the set of all $x \in A$ such that $f(x) \in E$. We call $f^{-1}(E)$ the **inverse image** of $E$ under *f*. If $y \in B$, $f^{-1}(y)$ is the set of all $x \in A$ such that $f(x) = y$. If, for each $y \in B$, $f^{-1}(y)$ consists of at most one element of A, then $f$ is said to be a 1-1 (*one-to-one*) mapping of $A$ into $B$. This may also be expressed as follows: $f$ is a 1-1 mapping of $A$ into $B$ provided that $f(x_1) \ne f(x_2)$ whenever $x_1 \ne x_2$, $x_1 \in A$, $x_2 \in A$.

### 2.3 Definition
If there exists a 1-1 mapping of $A$ onto $B$, we say that $A$ and $B$ can be put in 1-1 **correspondence**, or that $A$ and $B$ have the same **cardinal number**, or, briefly, that $A$ and $B$ are **equivalent**, and we write $A \sim B$. This relation clearly has the following properties:
+ It is reflexitive: $A \sim B$.
+ It is symmetric: If $A \sim B$, then $B \sim A$.
+ It is transitive: If $A \sim B$ and $B \sim C$, then $A \sim C$.

### 2.4 Definition
For any positive integer $n$, let $J_n$ be the set whose elements are the integers $1, 2, ..., n$; let $J$ be the set consisting of all positive integers. For any set $A$, we say:
1. $A$ is **finite** if $A \sim J_n$ for some $n$ (the empty set is also considered to be finite).
2. $A$ is **infinite** if $A$ is not finite.
3. $A$ is **countable** if $A \sim J$.
4. $A$ is **uncountable** if A is neither finite nor countable.
5. $A$ is **at most countable** if $A$ is finite or countable.

Countable sets are sometimes called **enumerable**, or **denumerable**.

### 2.7 Definition
By a **sequence**, we mean a function $f$ defined on the set $J$ of all positive integers. If $f(n) = x_n$, for $n \in J$, it is customary to denote the sequence $f$ by the symbol ${x_n}$, or sometimes by $x_1, x_2, x_3, ...$. The values of $f$, that is, the elements $x_n$, are called the terms of the sequence. If $A$ is a set and if $x_n \in A$ for all $n \in J$, then {x_n} is said to be a *sequence in $A$*, or a *sequence of elements of $A$*.

## Metric Spaces

### 2.15 Definition
A set $X$, whose elements we shall call **points**, is said to be a **metric space** if with any points $p$ and $q$ of $X$ there is associated a real number $d(p, q)$, called the distance from $p$ to $q$, such that
1. $d(p, q) \gt 0$ if $p \neq q$; $d(p, p) = 0$;
2. $d(p, q) = d(q, p)$;
3. $d(p, q) \leq d(p, r) + d(r, q)$, for any $r \in X$.

Any function with these three properties is called a *distance function*, or a *metric*.

### 2.17 Definition
By the **segment** $(a, b)$ we mean the set of all real numbers $x$ such that $a < x < b$.

By the **interval** $[a, b]$ we mean the set of all real numbers $x$ such that $a \le x \le b$.

Occasionally we shall also encouter "half-open intervals" $[a, b)$ and $(a, b]$; the first consist of all $x$ such that $a \le x < b$, the second of all $x$ such that $a < x \le b$.

If $a_i < b_i$ for $i = 1, ..., k$, the set of all points $x = (x_1, ..., x_k)$ in $R^k$ whose coordinates satisfy the inequalities $a_i \le x_i \le b_i$ $(1 \le i \le k)$ is called a $k$-cell. Thus a $1$-cell is an interval, a $2$-cell is a rectangle, etc.

If $x \in R^k$ and $r > 0$, the **open**(or **closed**) **ball** $B$ with center at $x$ and radius $r$ is defined to be the set of all $y \in R^k$ such that $\left|y-x\right| < r$ (or $\left|y-x\right| \le r$).

We call a set $E \subset R^k$ **convex** if $\lambda x + (1-\lambda)y \in E$ whenever $x \in E$, $y \in E$, and $0 < \lambda < 1$.

### 2.18 Definition
Let $X$ be a metric space. All points and sets mentioned below are understood to be elements and subsets of $X$.
1. A **neighborhood** of p is a set $N_r(p)$ consisting of all $q$ such that $d(p, q) < r$, for some $r > 0$. The number $r$ is called the *radius* of $N_r(p)$.
2. A point $p$ is a **limit point** of the set $E$ if *every* neighborhood of $p$ contians a point $q \ne p$ such that $q \in E$.
3. If $p \in E$ and $p$ is not a limit point of $E$, then $p$ is called an **isolated point** of $E$.
4. $E$ is **closed** if every limit point of $E$ is a point of $E$.
5. A point $p$ is an **interior** point of $E$ if there is a neighborhood $N$ of $p$ such that $N \subset E$.
6. $E$ is **open** if every point of $E$ is an interior of $E$.
7. The **complement** of $E$ (denoted by $E^c$) is the set of all points $p \in X$ such that $p \notin E$.
8. $E$ is **perfect** if $E$ is closed and if every point of $E$ is a limit point of $E$.
9. $E$ is **bounded** if there is a real number $M$ and a point $q \in X$ such that $d(p, q) < M$ for all $p \in E$.
10. $E$ is **dense** in $X$ if every point of $X$ is a limit point of $E$, or a point of $E$ (or both).

### 2.23 Theorem 
A set $E$ is open if and only if its complement is closed.

**Corollary** A set $F$ is closed if and only if its complement is open.

### 2.26 Definition 
If X is a metric space, if $E \subset X$, and if $E'$ denotes the set of all limit points of $E$ in $X$, then the **closure** of $E$ is the set $\bar{E} = E \cup E'$.

### 2.27 Theorem
If $X$ is a metric space and $E \subset X$, then
1. $\bar{E}$ is closed,
2. $E = \bar{E}$ if and only if $E$ is closed,
3. $E \subset F$ for every closed set $F \subset X$ such that $\bar{E} \subset F$.

### 2.28 Theorem
Let $E$ be a nonempty set of real numbers which is bounded above. Let $y = \sup E$. Then $y \in \bar{E}$. Hence $y \in E$ if $E$ is closed.


## Compact Sets


### 2.31 Definition
By an **open cover** of a set $E$ in a metric space $X$ we mean a collection $\{G_\alpha\}$ of open subsets of $X$ such that $E \subset \cup_\alpha G_\alpha$.

### 2.32 Definition
A subset $K$ of a metric space $X$ is said to be **compact** if every open cover of $K$ contains a *finite* subcover.

### 2.39 Theorem 
Let $k$ be a positive integer. If $\{I_n\}$ is a sequence of k

### 2.40 Theorem 
Every $k$-cell is compact.

### 2.41 Theorem
If a set $E$ in $R^k$ has one of following three properties, then it has the other two:
1. $E$ is closed and bounded.
2. $E$ is compact.
3. Every infinite subset of $E$ has a limit point in $E$.

---


# 3 Numberical Sequences and Series


## Convergent Sequences


### 3.1 Definition
A sequence ${p_n}$ in a metric space X is said to **converge** if there is a point $p \in X$ with the following property: For every $\epsilon > 0$ there is an integer $N$ such that $n \ge N$ implies that $d(p_n, p) < \epsilon$. (Here $d$ denotes the distance in $X$.)

In this case we also say that $\{p_n\}$ converges to $p$, or that $p$ is the limit of $\{p_n\}$, and we write $p_n \to p$, or

$\lim\limits_{x \to \infty}p_n = p$.

If ${p_n}$ does not converge, it is said to **diverge**.

### 3.2 Theorem
Let $\{p_n\}$ be a sequence in a metric space $X$.
1. $\{p_n\}$ converges to $p \in X$ if and only if every neighborhood of $p$ contains $p_n$ for all but finitely many $n$.
2. If $p \in X$, $p' \in X$, and if $\{p_n\}$ converges to $p$ and to $p'$, then $p' = p$.
3. If $\{p_n\}$ converges, then $\{p_n\}$ is bounded.
4. If $E \subset X$ and if $p$ is a limit point of $E$, then there is a sequence $\{p_n\}$ in $E$ such that $p = \lim\limits_{x \to \infty}p_n$.

---


# 4 Continuity


## Limits of Functions


### 4.1 Definition 
Let $X$ and $Y$ be metric spaces; suppose $E \subset X$, $f$ maps $E$ into $Y$, and $p$ is a limit point of $E$. We write $f(x) \to q$ as $x \to p$, or 

$\lim_{x \to p} f(x) = q$

if there is a point $q \in Y$ with the following property: For every $\epsilon \gt 0$ there exists a $\delta \gt 0$ such that

$d_{r}(f(x), q) \lt \epsilon$

for all points $x \in E$ for which

$0 \lt d_{x}(x, p) \lt \delta$.

### 4.2 Theorem
Let $X$, $Y$, $E$, $f$, and $p$ be as in Definition 4.1. Then

$\lim\limits_{x \to p}f(x) = q$

if and only if

$\lim\limits_{x \to \infty}f(p_n) = q$

for every sequence{p_n} in $E$ such that

$p_n \ne p$, $\lim\limits_{x \to \infty}p_n = p$.

### 4.4 Theorem
Suppose $E \subset X$, a metric space, $p$ is a limit point of $E$, $f$ and $g$ are complex functions on $E$, and

$\lim\limits_{x \to p}f(x) = A$, $\lim\limits_{x \to p}g(x) = B$.

Then
1. $\lim\limits_{x \to p}(f+g)(x) = A + B$;
2. $\lim\limits_{x \to p}(fg)(x) = AB$;
3. $\lim\limits_{x \to p}(\frac{f}{g})(x) = \frac{A}{B}$, if $B \ne 0$.


## Continuous Functions

### 4.5 Definition
Suppose $X$ and $Y$ are metric spaces, $E \subset X$, $p \in E$, and $f$ maps $E$ into $Y$. Then $f$ is said to be **continuous** at $p$ if for every $\epsilon > 0$ there exists a $\delta > 0$ such that 

$d_Y(f(x), f(p) < \epsilon$

for all points $x \in E$ for which $d_X(x, p) < \delta$.

If $f$ is continuous at every point of E, then f is said to be continuous on $E$.


## Continuity and Compactness

### 4.13 Definition
A mapping $\mathbf{f}$ of a set $E$ into $R^k$ is said to be **bounded** if there is a real number $M$ such that $\left|\mathbf{f}(x)\right| \le M$ for all $x \in E$.

### 4.15 Theorem
If $\mathbf{f}$ is a continuous mapping of a compact metric space $X$ into $R^k$, then $\mathbf{f}(X)$ is closed and bounded. Thus, $\mathbf{f}$ is bounded.

### 4.16 Theorem
Suppose $f$ is a continuous real function on a compact metric space X, and

$M = \sup\limits_{p \in x} f(p)$, $m = \inf\limits_{p \in X} f(p)$.

Then there exist point $p, q \in X$ such that $f(p) = M$ and $f(q) = m$.

### 4.33 Definition
Let $f$ be a real function defined on $E \subset R$. We say that

$f(t) \to A$ as $t \to x$,

where $A$ and $x$ are in the extended real number system, if for every neighborhood $U$ of $A$ there is a neighborhood $V$ of $x$ such that $V \cap E$ is not empty, and such that $f(t) \in U$ for all $t \in V \cap E$, $t \ne x$.

---

# 5 Differentiation


## The Derivative of a Real Function


### 5.1 Definition
Let $f$ be defined (and real-valued) on $[a, b]$. For any $x \in [a, b]$ form the quotient

(1) $\phi(t) = \frac{f(t) - f(x)}{t - x}$ $(a < t < b, t \ne x)$,

and define

(2) $f'(x) = \lim_{t \to x}\phi(t)$,

provided this limit exists in accordance with Definition 4.1.

We thus associate with the function $f$ a function $f'$ whose domain is the set of points $x$ at which (2) exists; $f'$ is called the *derivative* of $f$.

If $f'$ is defined at a point x, we say that f is *differentiable* at $x$. If $f'$ is defined at every point of a set $E \subset [a, b]$, we say that $f$ is differentiable on E.

It is possible to consider right-hand and left-hand limits in (2); this leads to the definition of right-hand and left-hand derivatives. In particular, at the endpoints $a$ and $b$, the derivative, if it exists, is a right-hand or left-hand derivative, respectively. We shall not, however, discuss one-sided derivatives in any detail.

If $f$ is defined on a segment $(a, b)$ and if $a < x < b$, then $f'(x)$ is defined by (1) and (2), as above. but $f'(a)$ and $f'(b)$ are not defined in this case.

### 5.2 Theorem
Let f be defined on $[a, b]$. If $f$ is differentiable at a point $x \in [a, b]$, then $f$ is *continuous* at $x$.

### 5.3 Theorem
Suppose $f$ and $g$ are defined on $[a, b]$ and are differentiable at a point $x \in [a, b]$. Then $f + g$, $fg$, and $f/g$ are differentiable at $x$, and
1. $(f+g)'(x) = f'(x) + g'(x)$;
2. $(fg)'(x) = f'(x)g(x) + f(x)g'(x)$;
3. $(f/g)'(x) = \frac{(g(x)f'(x) - g'(x)f(x)}{g^2(x)}$

In 3, we assume of course that $g(x) \ne 0$.

## Mean Value Theorems

### 5.7 Definition
Let $f$ be a real function on a metric space $X$. We say that $f$ has a **local maximum** at a point $p \in X$ if there exists $\delta > 0$ such that $f(q) \le f(p)$ for all $q \in X$ with $d(p, q) < \delta$.

Local minima are defined likewise.

### 5.8 Theorem
Let $f$ be defined on $[a, b]$; if $f$ has a local maximum at a point $x \in (a, b)$, and if $f'(x)$ exists, then $f'(x) = 0$.

### 5.9 Theorem **Generalized Mean Value Theorems**
If $f$ and $g$ are continuous real functions on $[a, b]$ which are differentiable in $(a, b)$, then there is a point $x \in (a, b)$ at which

$[f(b)-f(a)]g'(x) = [g(b)-g(a)]f'(x)$.

Note that differntiability is not required at the endpoints.

**Proof:** Put

$h(t) = [f(b)-f(a)]g(t) - [g(b)-g(a)]f(t)$, $(a \le t \le b)$.

Then $h$ is continuous on $[a, b]$, $h$ is differentiable in $(a, b)$, and

$h(a) = f(b)g(a) - f(a)g(b) = h(b)$.

To prove the theorem, we have to show that $h'(x) = 0$ for some $x \in (a, b)$.

If $h$ is constant, this holds for every $x \in (a, b)$. If $h(t) > h(a)$ for some $t \in (a, b)$, let $x$ be a point on $[a, b]$ at which $h$ attains its maximum
