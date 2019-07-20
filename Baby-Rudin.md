# 1 The Real and Complex Number Systems


## Introduction

### 1.3 Definition
If $A$ is any set (whose elements may be numbers or any other objects), we write $x \in A$ to indicate that $x$ is a member (or an element) of $A$.

If $x$ is not a member of $A$, we write: $x \notin A$.

The set which contains no element will be called the **empty set**. If a set has at least one element, it is called **nonempty**.

If $A$ and $B$ are sets, and if every element of $A$ is an element of $B$, we say that $A$ is a subset of $B$, and write $A \subset B$, or $B \supset A$. If, in addtion, there is an element of $B$ which is not in $A$, then $A$ is said to be a **proper** subset of $B$. Note that $A \subset A$ for every set $A$.

If $A \subset B$ and $B \subset A$, we write $A = B$. Otherwise $A \ne B$.


## Ordered Sets

### 1.5 Definition
Let $S$ be a set. An **order** on $S$ is a relation, denoted by $<$, with the following two properties:

1. If $x \in S$ and $y \in S$ then one and only one of the satements $x < y$, $x = y$, $x > y$ is true.
2. If $x, y, z \in S$, If $x < y$ and $y < z$, then $x < z$.

The statement "$x < y$" may be read as "$x$ is less than $y$" or "$x$ is smaller then $y$" or "$x$ precedes $y$".

It is often convenient to write $y > x$ in place of $x < y$.

The notation $x \ne y$ indicates that $x < y$ or $x = y$, without specifying which of these two is to hold. In other world, $x \ne y$ is the negation of $x > y$.

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


### 1.10 Definition
An ordered set $S$ is said to have the **least-upper-bound property** if the following is true:

If $E \subset S$, $E$ is not empty, and $E$ is bounded above, then sup $E$ exists in $S$.

### 1.11 Theorem
Suppose $S$ is an ordered set with the least-upper-bound property, $B \subset S$, $B$ is not empty, and $B$ is bounded below. Let $L$ be the set of all lower bounds of $B$. Then

$\alpha = \sup L$

exists in $S$, and $\alpha = \inf B$.

In particular, $\inf B$ exists in $S$.


## Fields

### 1.12 Definition
A **field** is a set $F$ with two operations, called **addition** and **multiplication**, which satisfy the following so-called "field axioms" (A), (M), and (D):

#### (A) Axioms for addition
1. If $x \in F$ and $y \in F$, then their sum $x + y$ is in $F$.
2. Addition is commutative: $x + y = y + x$ for all $x, y \in F$.
3. Addition is associative: $(x + y) + z = x + (y + z)$ for all $x, y, z \in F$.
4. $F$ contains an element $0$ such that $0 + x = x$ for every $x \in F$.
5. To every $x \in F$ corresponds an element $-x \in F$ such that $x + (-x) = 0$.

#### (M) Axioms for multiplication
1. If $x \in F$ and $y \in F$, then their product $xy$ is in $F$.
2. Multiplication is commutative: $xy = yx$ for all $x, y \in F$.
3. Multiplication is associative: $(xy)z = x(yz)$ for all $x, y, z \in F$.
4. $F$ contains an element $1 \ne 0$ such that $1x = x$ for every $x \in F$.
5. If $x \in F$ and $x \ne 0$ then there exists an element $1/x \in F$ such that $x\cdot(1/x) = 1$.

#### (D) The Distributive Law 
$x(y + z) = xy + xz$ holds for all $x, y, z \in F$.


### 1.14 Proposition
The axioms for addition imply the following statements.
1. If $x + y = x + z$ then $y = z$.
2. If $x + y = x$ then $y = 0$.
3. If $x + y = 0$ then $x = -x$.
4. $-(-x) = x$.

### 1.15 Proposition
The axioms for multiplication imply the following statements.
1. If $x \ne 0$ and $xy = xz$ then $y = z$.
2. If $x \ne 0$ and $xy = x$ then $y = 1$.
3. If $x \ne 0$ and $xy = 1$ then $y = 1/x$.
4. If $x \ne 0$ then $1/(1/x) = x$.

### 1.16 Proposition
The field axioms imply the following statements, for any $x, y, z \in F$.
1. 0x = 0.
2. If $x \ne 0$ and $y \ne 0$ then $xy \ne 0$.
3. $(-x)y = -(xy) = x(-y)$.
4. $(-x)(-y) = xy$.

### 1.17 Definition
An **ordered field** is a **field** $F$ which is also an **ordered set**, such that
1. $x + y < x + z$ if $x, y, z \in F$ and $y < z$,
2. $xy > 0$ If $x \in F$, $y \in F$, $x > 0$, and $y > 0$.

If $x > 0$, we call x **positive**; if $x < 0$, $x$ is **negative**.

### 1.18 Proposition
The following statements are true in every ordered field.
1. If $x > 0$ then $-x < 0$, and vice versa.
2. If $x > 0$ and $y < z$ then $xy < xz$.
3. If $x < 0$ and $y < z$ then $xy > xz$.
4. If $x \ne 0$ then $x^2 > 0$. In particular, $1 > 0$.
5. If $0 < x < y$ then $0 < 1/y < 1/x$.


## The Real Field


### 1.20 Theorem
1. If $x \in R$, $y \in R$, and $x > 0$, then there is a positive integer $n$ such that $nx > y$.
2. If $x \in R$, $y \in R$, and $x < y$, then there exists a $p \in Q$ such that $x < p < y$.

Part 1 is usually referred to as the **archimedean property** of $R$. Part 2. may be stated by saying that $Q$ is dense in $R$: Between any two real numbers there is a rational one.


## The Extended Real Number System


### 1.23 Definition 
The extended real number system consists of the real field R and two symbols, $+\infty$ and $-\infty$. We preserve the original order in R, and define

$-\infty < x < +\infty$

for every $x \in R$.

It is then clear that $+\infty$ is an upper bound of every subset of the extended real number system, and that every nonempty subset has a leat upper bound. If, for example, $E$ is a nonempty set of real numbers which is not bounded above in R, then sup $E = +\infty$ in the extended real number system.

Exactly the same remarks apply to lower bounds.

The extended real number system does not form a field, but it is customary to make the following conventions:
1. If $x$ is real then $x+\infty=+\infty$, $x-\infty=-\infty$, $\frac x {+\infty} = \frac x {-\infty} = 0$.
2. If $x > 0$ then $x \cdot (+\infty) = +\infty$, $x \cdot (-\infty) = -\infty$.
3. If $x < 0$ then $x \cdot (+\infty) = -\infty$, $x \cdot (-\infty) = +\infty$.

When it is desired to make the distinction between real numbers on the one hand the symbols $+\infty$ and $-\infty$ on the other quite explicit, the former are called **finite**.


## Appendix **Construct $R$ from $Q$**
### Step 1 
The members of $R$ will be certain subset of $Q$, called **cuts**. A cut is, by definition, any set $\alpha \subset Q$ with the following three properties.
1. $\alpha$ is not empty, and $\alpha \ne Q$.
2. If $p \in \alpha$, $q \in Q$, and $q < p$, then $q \in \alpha$.
3. If $p \in \alpha$, then $p < r$ for some $r \in alpha$.

The letters $p, q, r, \dots$ will always denote rational numbers, and $\alpha, \beta, \gamma, \dots$ will denote cuts.

### Step 2
Define "$\alpha < \beta$" to mean: $\alpha$ is a proper subset of $\beta$.

### Step 3
The ordered set $R$ has the least-upper-bound property.

### Step 4
If $\alpha \in R$ and $\beta \in R$ we define $\alpha + \beta$ to be the set of all sums $r + s$, where $r \in \alpha$ and $s \in \beta$.

### Step 5



# 2 Basic Topology


## Finite, Countable, and Uncountable Sets


### 2.1 Definition
Consider two set $A$ and $B$, whose elements may be any objects whatsoever, and suppose that with each element $x$ of $A$ there is associated, in some manner, an elment of $B$, which we denote by $f(x)$. Then $f$ is said to be a **function** from $A$ to $B$ (or a **mapping** of A into B). The set $A$ is called the **domain** of $f$ (we also say $f$ is defined on $A$), and the elements $f(x)$ are called the **values** of $f$. The set of all values of $f$ is called the **range** of $f$.

### 2.2 Definition
Let $A$ and $B$ be two sets and let $f$ be a mapping of $A$ into $B$. If $E \subset A$, $f(E)$ is defined to be the set of all elements $f(x)$, for $x \in E$. We call $f(E)$ the **image** of $E$ under $f$. In this notation, $f(A)$ is the range of $f$. It is clear that $f(A) \subset B$. If $f(A) = B$, we say that $f$ maps $A$ **onto** $B$. (Note that, according to this usage, **onto** is more specific than **into**.)

If $E \subset B$, $f^{-1}(E)$ denotes the set of all $x \in A$ such that $f(x) \in E$. We call $f^{-1}(E)$ the **inverse image** of $E$ under *f*. If $y \in B$, $f^{-1}(y)$ is the set of all $x \in A$ such that $f(x) = y$. If, for each $y \in B$, $f^{-1}(y)$ consists of at most one element of A, then $f$ is said to be a 1-1 (*one-to-one*) mapping of $A$ into $B$. This may also be expressed as follows: $f$ is a 1-1 mapping of $A$ into $B$ provided that $f(x_1) \ne f(x_2)$ whenever $x_1 \ne x_2$, $x_1 \in A$, $x_2 \in A$.

### 2.3 Definition
If there exists a 1-1 mapping of $A$ onto $B$, we say that $A$ and $B$ can be put in 1-1 **correspondence**, or that $A$ and $B$ have the same **cardinal number**, or, briefly, that $A$ and $B$ are **equivalent**, and we write $A \sim B$. This relation clearly has the following properties:
+ It is reflexitive: $A \sim A$.
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
By a **sequence**, we mean a function $f$ defined on the set $J$ of all positive integers. If $f(n) = x_n$, for $n \in J$, it is customary to denote the sequence $f$ by the symbol ${x_n}$, or sometimes by $x_1, x_2, x_3, ...$. The values of $f$, that is, the elements $x_n$, are called the terms of the sequence. If $A$ is a set and if $x_n \in A$ for all $n \in J$, then $\{x_n\}$ is said to be a **sequence in $A$**, or a **sequence of elements of $A$**.

### 2.8 Theorem
Every infinite subset of a countable set $A$ is countable.

### 2.9 Definition
Let $A$ and $\Omega$ be sets, and suppose that with each element $\alpha$ of $A$ there is associated a subset of $\Omega$ which we denote by $E_\alpha$.

The set whose elements are the set $E_\alpha$ will be denoted by $\{E_\alpha\}$. Instead of speaking of sets of sets, we shall sometimes speak of a cllection of sets, or a family of sets.

The **union** of the sets $E_\alpha$ is defined to be the set $S$ such that $x \in S$ if and only if $x \in E_\alpha$ for at least one $\alpha \in A$. We use the notaiton
$$
S = \bigcup_{\alpha \in A}E_\alpha.
$$
If $A$ consists of the integers $1, 2, \dots, n,$ one usually writes
$$
S = \bigcup_{m = 1}^n E_m.
$$
or
$$
S = E_1 \cup E_2 \cup \cdots \cup E_n.
$$
If $A$ is the set of all positive integers, the usual notaiton is
$$
S = \bigcup_{m = 1}^\infty E_m
$$
The symbol $\infty$ indicates that the union of a **countable** collection of sets is taken, and should not be confused with the symbols $+\infty$, $-\infty$.

The **intersection** the sets $E_\alpha$ is defined to be the set $P$ such that $x \in P$ if and only if $x \in E_\alpha$ for every $\alpha \in A$. We use the notation
$$
P = \bigcap_{\alpha \in A}E_\alpha,
$$
or
$$
P = \bigcap_{m=1}^n E_m = E_1 \cap E_2 \cap \cdots \cap E_n,
$$
or
$$
P = \bigcap_{m=1}^\infty E_m.
$$
as for unions. If $A \cap B$ is not empty, we say that $A$ and $B$ **intersect**; otherwise they are **disjoint**.

### 2.12 Theorem
Let $\{E_n\}, n = 1, 2, 3, \dots,$ be a sequence of countable sets, and put
$$
S = \bigcup_{n=1}^\infty E_n
$$
Then $S$ is countable.

**Corollary** Suppose $A$ is at most countable, and, for every $\alpha \in A$, $B_\alpha$ is at most countable. Put
$$
T = \bigcup_{\alpha \in A}B_\alpha.
$$
Then $T$ is at most countable.

### 2.13 Theorem
Let $A$ be a countable set, and let $B_n$ be the set of all $n$-tuples $(a_1, \dots, a_n)$, where $a_k \in A (k = 1, \dots, n)$, and the elements $a_1, \dots, a_n$ need not be distinct. Then $B_n$ is countable.

**Corollary** The set of all rational numbers is countable.

### 2.14 Theorem
Let $A$ be the set of all sequences whose elements are the digits $0$ and $1$. This set $A$ is uncountable.

The elements of $A$ are sequences like $1, 0, 0, 1, 0, 1, 1, 1, \dots$.

**Proof** Let $E$ be a countable subset of $A$, and let $E$ consist of the sequences $s_1, s_2, s_3, \dots$ We construct a sequence $s$ as follows. If the $n$th digit in $s_n$ is $1$, we let the $n$th digit of $s$ be 0, and vice versa. Then the sequence $s$ differs from every member of $E$ in at least one place; hence $s \notin E$. But clearly $s \in A$, so that $E$ is a proper subset of $A$.

We have shown that every countable subset of$A$ is a proper subset of $A$. It follows that $A$ is uncountable (for otherwise $A$ would be a proper subset of A, which is absurd).

The idea of above proof was first used by Cantor, and is called Cantor's diagonal process.


## Metric Spaces

### 2.15 Definition
A set $X$, whose elements we shall call **points**, is said to be a **metric space** if with any points $p$ and $q$ of $X$ there is associated a real number $d(p, q)$, called the distance from $p$ to $q$, such that
1. $d(p, q) \gt 0$ if $p \neq q$; $d(p, p) = 0$;
2. $d(p, q) = d(q, p)$;
3. $d(p, q) \leq d(p, r) + d(r, q)$, for any $r \in X$.

Any function with these three properties is called a **distance function**, or a **metric**.

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

### 2.19 Theorem
Every neighborhood is an open set.

### 2.20 Theorem
If $p$ is a limit point of a set $E$, then every neighborhood of $p$ contains infinitely many points of $E$.

**Corollary** A finite point set has no limit point.

### 2.22 Theorem
Let $\{E_\alpha\}$ be a (finite or infinite) collection of sets $E_\alpha$. Then
$$
(\bigcup_\alpha E_\alpha)^c = \bigcap_\alpha(E_\alpha^c).
$$

### 2.23 Theorem 
A set $E$ is open if and only if its complement is closed.

**Corollary** A set $F$ is closed if and only if its complement is open.

### 2.24 Theorem
1. For any collection $\{G_\alpha\}$ of open sets, $\cup_\alpha G_\alpha$ is open.
2. For any collection $\{F_\alpha\}$ of closed sets, $\cap_\alpha F_\alpha$ is closed.
3. For any finite collection $G_1, G_2, \dots, G_n$ of open sets, $\cap_{i=1}^nG_i$ is open.
4. For any finite collection $F_1, F_2, \dots, F_n$ of closed sets, $\cup_{i=1}^nF_i$ is closed.

### 2.26 Definition 
If X is a metric space, if $E \subset X$, and if $E'$ denotes the set of all limit points of $E$ in $X$, then the **closure** of $E$ is the set $\bar{E} = E \cup E'$.

### 2.27 Theorem
If $X$ is a metric space and $E \subset X$, then
1. $\bar{E}$ is closed,
2. $E = \bar{E}$ if and only if $E$ is closed,
3. $\bar{E} \subset F$ for every closed set $F \subset X$ such that $E \subset F$.

### 2.28 Theorem
Let $E$ be a nonempty set of real numbers which is bounded above. Let $y = \sup E$. Then $y \in \bar{E}$. Hence $y \in E$ if $E$ is closed.

### 2.29 Remark
Suppose $E \subset Y \subset X$, where $X$ is a metric space. To say that $E$ is an open subset of $X$ means that to each point $p \in E$ there is associated a positive number $r$ such that the conditions $d(p, q) < r, q \in X$ imply that $q \in E$. $Y$ is also a metric space, so that our definitions may equally well be made within $Y$. To be quite explicit, let us say that $E$ is **open relative** to $Y$ if to each $p \in E$ there is associate an $r > 0$ such that $q \in E$ whenever $d(p, q) < r$ and $q \in Y$.A set may be open relative to $Y$ without being an open subset of $X$.

### 2.30 Theorem
Suppose $Y \subset X$. A subset $E$ of $Y$ is open relative to $Y$ if and only if $E = Y \cap G$ for some open subset $G$ of $X$.


## Compact Sets


### 2.31 Definition
By an **open cover** of a set $E$ in a metric space $X$ we mean a collection $\{G_\alpha\}$ of open subsets of $X$ such that $E \subset \bigcup_\alpha G_\alpha$.

### 2.32 Definition
A subset $K$ of a metric space $X$ is said to be **compact** if every open cover of $K$ contains a *finite* subcover.

### 2.33 Theorem
Suppose $K \subset Y \subset X$. Then $K$ is compact relative to $X$ if and only if $K$ is compact relative to $Y$.

By virtue of this theorem we are able, in many situations, to regard compact sets as metric spaces in their own right, without paying any attention to any embedding space. In particular, although it makes little sense to talk of **open** spaces, or of **closed** spaces (every metric space $X$ is an open subset of itself, and is a closed subset of itself), it does make sense to talk of **compact** metric spaces.

### 2.34 Theorem
Compact subsets of metric spaces are closed.

### 2.35 Theorem
Closed subsets of compact sets are compact.

**Proof** Suppose $F \subset K \subset X$, $F$ is closed (relative to $X$), and $K$ is compact. Let $\{V_\alpha\}$ be an open cover of $F$. If $F^c$ is adjoined to $\{V_\alpha\}$, we obtain an open cover $\Omega$ of $K$. Since $K$ is compact, there is a finite subcollection $\Phi$ of $\Omega$ which covers $K$, and hence $F$. If $F^c$ is a member of $\Phi$, we may remove it from $\Phi$ and still retain an open cover of $F$. We have thus shwn that a finite subcollection of $\{V_\alpha\}$ covers $F$.

**Corollary** If $F$ is closed and $K$ is compact then $F \cap K$ is compact.

### 2.36 Theorem
If $\{K_\alpha\}$ is a collection of compact subsets of a metric space $X$ such that the intersection of every finite subcollection of $\{K_\alpha\}$ is nonempty, then $\cap K_\alpha$ is nonempty.

**Corollary** If $\{K_n\}$ is a sequence of nonempty compact sets such that $K_n \supset K_{n+1} (n = 1, 2, 3, \dots)$, then $\cap_1^\infty K_n$ is not empty.

### 2.37 Theorem
If $E$ is an infinite subset of a compact set $K$, then $E$ has a limit point in $K$.

### 2.38 Theorem
If $\{I_n\}$ is a sequence of intervals in $R^1$, such that $I_n \supset I_{n+1}$ $(n = 1,2,3,...)$, then $\bigcap_1^\infty I_n$ is not empty.

### 2.39 Theorem 
Let $k$ be a positive integer. If $\{I_n\}$ is a sequence of $k$-cells such that $I_n \supset I_{n+1}$ $(n = 1,2,3,...)$, then $\bigcap_1^\infty I_n$ is not empty.

### 2.40 Theorem 
Every $k$-cell is compact.

### 2.41 Theorem
If a set $E$ in $R^k$ has one of following three properties, then it has the other two:
1. $E$ is closed and bounded.
2. $E$ is compact.
3. Every infinite subset of $E$ has a limit point in $E$.

### 2.42 Theorem (Weierstrass)
Every bounded infinite subset of $\{R^k\}$ has a limit point in $R^k$.


## Perfect Sets

### 2.43 Theorem


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


## Subsequences


### 3.5 Definition
Given a sequence $\{p_n\}$, consider a sequence $\{n_k\}$ of positive integers, such that $n_1 < n_2 < n_3 < \cdots$. then the sequence $\{p_{n_i}\}$ is called a **subsequence** of $\{p_n\}$. If $\{p_{n_i}\}$ converges, its limit is called a **subsequential limit** of $\{p_n\}$.


### 3.7 Theorem
The subsequential limits of a sequence $\{p_n\}$ in a metric space $X$ form a closed subset of $X$.


## Cauchy Sequences

### 3.8 Definition
A sequence $\{p_n\}$ in a metric space X is said to be a **Cauchy sequence** if for every $\epsilon > 0$ there is an integer $N$ such that $d(p_n, p_m) < \epsilon$ if $n \ge N$ and $m \ge N$.

### 3.9 Definition
Let $E$ be a nonempty subset of a metric space $X$, and let $S$ be the set of all real numbers of the form $d(p, q)$, with $p \in E$ and $q \in E$. The sup of $S$ is called the **diameter** of $E$.

If $\{p_n\}$ is a sequence in $X$ and if $E_N$ consists of the points $p_N, p_{N+1}, p_{N+2}, \dots$, it is clear from the two preceding definitions that $\{p_n\}$ is a Cauchy sequence if and only if
$$
\lim_{N \to \infty} \mathop{diam} E_N = 0.
$$

### 3.10 Theorem
1. If $\bar{E}$ is the closure of a set $E$ in a metric space $X$, then $diam \bar{E}$ = diam E$.
2. If $K_n$ is a sequence of compact sets in $X$ such that $K_n \supset K_{n+1}$ $(n = 1,2,3,\dots)$ and if $\lim\limits_{n \to \infty} diam K_n = 0$, then $\bigcap_1^{\infty}K_n$ consists of exactly one point.($K_n$ must not be empty set)

### 3.11 Theorem
1. In any metric space $X$, every convergent sequence is a Cauchy sequence.
2. If $X$ is a compact metric space and if $\{p_n\}$ is a Cachy sequence in $X$, then $\{p_n\}$ converges to some point of $X$.
3. In $R^k$, every Cauchy sequence converges.

### 3.12 Definition
A metric space in which every Cauchy sequence converges is said to be **complete**.

### 3.13 Definition 
A sequence $\{s_n\}$ of real numbers is said to be
1. **monotonically increasing** if $s_n \le s_{n+1} (n = 1, 2, 3, \dots)$;
2. **monotonically decreasing** if $s_n \ge s_{n+1} (n = 1, 2, 3, \dots)$.

The class of monotonic sequences consists of the increasing and the decreasing sequences.

### 3.14 Theorem
Suppose $\{s_n\}$ is monotonic. Then $\{s_n\}$ converges if and only if it is bounded.


## Upper and Lower Limits


### 3.15 Definition 
Let $\{s_n\}$ be a sequence of real numbers with the following property: For every real $M$ there is an integer $N$ such that $n \ge N$ implies $s_n \ge M$. We then write

$s_n \to +\infty$.

Similarly, if for every real $M$ there is an integer $N$ such that $n \ge N$ implies $s_n \le M$, we write

$s_n \to -\infty$.


### 3.16 Definition
Let $\{s_n\}$ be a sequence of real numbers. Let $E$ be the set of numbers $x$ (in the extended real number system) such that $s_{n_k} \to x$ for some subsequence $\{s_{n_k}\}$. This set $E$ contains all subsequential limits as defined in Definition 3.5, plus possibly the numbers $+\infty$, $-\infty$.

We now recall Definition 1.8 and Definition 1.23 and put

$s^* = \sup E$,

$s_* = \inf E$.

The numbers $s^*$, $s_*$ are called the **upper limit** and **lower limit** of $\{s_n\}$; we use the notation

$\mathop{\lim \sup}\limits_{n \to \infty} s_n = s^*$, $\mathop{\lim \inf}\limits_{n \to \infty} s_n = s_*$.


### 3.17 Theorem
Let $\{s_n\}$ be a sequence of real numbers. Let $E$ and $s^*$ have the same meaning as in Definition 3.16. Then $s^*$ has the following two properties:
1. $s^* \in E$.
2. If $x > s^*$, there is a integer $N$ such that $n \ge N$ implies $s_n < x$.

Moreover, $s^*$ is the only number with the properties 1 and 2.

Of course, an analogous result is true for $s_*$.


## Series


### 3.21 Definition
Given a sequence $\{a_n\}$, we use the notation

$\sum\limits_{n = p}^q a_n$ $(p \le q)$

to denote the sum $a_p + q_{p+1} + ... + a_q$. With $\{a_n\}$ we associate a sequence $\{s_n\}$, where

$s_n = \sum\limits_{k=1}^n a_k$.

For $\{s_n\}$ we also use the symbolic expression

$a_1 + a_2 + a_3 + ...$

or, more concisely,

**(Symbol Series 1)** $\sum\limits_{n=1}^\infty a_n$.

The (Symbol Series) we call an **infinite series**, or just a **series**. The numbers $s_n$ are called the **partial sums** of the series. If $\{s_n\}$ converges to $s$, we say that the series **converges**, and write

$\sum\limits_{n=1}^\infty a_n = s$.

The number $s$ is called the sum of the series; but it should be clearly understood that $s$ is the limit of a sequence of sums, and is not obtained simply by addition.

If $\{s_n\}$ diverges, the series is saied to diverge.

Sometimes for convenience of notation, we shall consider series of the form

**(Symbol Series 2)** $\sum\limits_{n=0}^\infty a_n$.

And frequently, when there is no possible ambiguity, or when the distinction is immaterial, we shall simply write $\sum a_n$ in place of (Symbol Series 1) or (Symbol Series 2).

### 3.22 Theorem
$\sum a_n$ converges if and only if for every $\epsilon > 0$ there is an integer $N$ such that
$$
|\sum_{k=n}^m a_k| \le \epsilon
$$
if $m \ge n \ge N$.

In paritcular, by taking $m = n$, it becomes
$$
|a_n| < \epsilon (n \ge N).
$$

### 3.23 Theorem 
If $\sum a_n$ converges, then $\lim_{n \to \infty}a_n = 0$.

### 3.24 Theorem
A series of nonnegative terms converges if and only if its partial sums form a bounded sequence.

### 3.25 Theorem **Comparasion Test**
1. If $|a_n| \le c_n$ for $n \ge N_0$, where $N_0$ is some fixed integer, and if $\sum c_n$ converges, then $\sum a_n$ converges.
2. If $a_n \ge d_n \ge 0$ for $n \ge N_0$, and if $\sum d_n$ diverges, then $\sum a_n$ diverges.



## The Root and Ratio Tests


### 3.33 Theorem **Root Test**
Given $\sum a_n$, put $\alpha = \mathop{\lim \sup}\limits_{n \to \infty}\sqrt[n]{\left|a_n\right|}$.

Then
1. if $\alpha < 1$, $\sum a_n$ converges;
2. if $\alpha > 1$, $\sum a_n$ diverges;
3. if $\alpha = 1$, the test gives no information.


### 3.34 Theorem **Ratio Test**
The series $\sum a_n$
1. converges if $\mathop{\lim \sup}\limits_{n \to \infty} \lvert\frac {a_{n+1}} {a_n}\rvert < 1$,
2. diverges if $\frac {a_{n+1}} {a_n} \ge 1$ for all $n \ge n_0$, where $n_0$ is some fixed integer.


## Power Series


### 3.38 Definition
Given a sequence $\{c_n\}$ of complex numbers, the series

$\sum\limits_{n=0}^\infty c_nz^n$

is called a **power series**. The numbers $c_n$ are called the coefficients of the series; $z$ is a complex number.

### 3.39 Theorem
Given the power series $\sum c_n z^n$, put

$\alpha = \mathop{\lim \sup}\limits_{n \to \infty} \sqrt[n]{\left|c_n\right|}$, $R = \frac 1 \alpha$

(If $\alpha = 0$, $R = +\infty$; if $\alpha = +\infty$, $R = 0$) Then $\sum c_n n^z$ converges if $|z| < R$, and diverges if $|z| > R$.

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

$d_Y(f(x), f(p)) < \epsilon$

for all points $x \in E$ for which $d_X(x, p) < \delta$.

If $f$ is continuous at every point of E, then f is said to be **continuous** on $E$.

### 4.6 Theorem
In the situation given in Definition 4.5, assume also that $p$ is a limit point of $E$. Then $f$ is continuous at $p$ if and only if $\lim_{x \to p}f(x) = f(p))$.

### 4.7 Theorem
Suppose $X$, $Y$, $Z$ are metric spaces, $E \subset X$, $f$ maps $E$ into $Y$, $g$ maps the range of $f$, $f(E)$, into $Z$, and h is the mapping of $E$ into $Z$ defined by

$h(x) = g(f(x))$ $(x \in E)$.

If $f$ is coninuous at a point $p \in E$ and if $g$ is continuous at the point $f(p)$, then $h$ is continuous at $p$.

This function $h$ is called the **composition** or the **composite** of $f$ and $g$. The notation

$h = g \circ f$

is frequently used in this context.

### 4.9 Theorem
Let $f$ and $g$ be complex continuous functions on a metric space $X$. Then $f+g$, $fg$, and $f/g$ are continuous on $X$.

In the last case, we must of course assume that $g(x) \ne 0$, for all $x \in X$.


## Continuity and Compactness

### 4.13 Definition
A mapping $\mathbf{f}$ of a set $E$ into $R^k$ is said to be **bounded** if there is a real number $M$ such that $\left|\mathbf{f}(x)\right| \le M$ for all $x \in E$.

### 4.15 Theorem
If $\mathbf{f}$ is a continuous mapping of a compact metric space $X$ into $R^k$, then $\mathbf{f}(X)$ is closed and bounded. Thus, $\mathbf{f}$ is bounded.

### 4.16 Theorem
Suppose $f$ is a continuous real function on a compact metric space X, and

$M = \sup\limits_{p \in x} f(p)$, $m = \inf\limits_{p \in X} f(p)$.

Then there exist point $p, q \in X$ such that $f(p) = M$ and $f(q) = m$.


### 4.18 Definition
Let $f$ be a mapping of metric space $X$ into a metric space $Y$. We say that $f$ is **uniformly continuous** on $X$ if for every $\epsilon > 0$ there exists $\delta > 0$ such that

**(equation 4.15)**
$$ d_Y(f(p), f(q)) < \epsilon $$
for all $p$ and $q$ in $X$ for which $d_X(p, q) < \delta$.

### 4.19 Theorem
Let $f$ be a continuous mapping of a compact metric space $X$ into a metric space $Y$. Then $f$ is uniformly continuous on $X$.



## Discontinuities


### 4.25 Definition
Let $f$ be defined on $(a, b)$. Consider any point $x$ such that $a \le x < b$. We write 
$$f(x+) = q$$
if $f(t_n) \to q$ as $n \to \infty$, for all sequences $\{t_n\}$ in $(x, b)$ such that $t_n \to x$. To obtain the definition of $f(x-), for $a < x \le b$, we restrict ourselves to sequences $\{t_n\}$ in (a, x).

It is clear that any point $x$ of $(a, b)$, $\lim_{t \to x}f(t)$ exists if and only if
$$ f(x+) = f(x-) = \lim_{t \to x}f(t) $$

### 4.26 Definition
Let $f$ be defined on $(a, b)$. If $f$ is discontinuous at a point $x$, and if $f(x+)$ and $f(x-)$ exist, then $f$ is said to have a discontinuity of the **first kind**, or a **simple discontinuity**, at $x$. Otherwise the discontinuity is said to be a **second kind**.



## Monotonic Functions


### 4.28 Definition
Let $f$ be real on $(a, b)$. Then $f$ is said to be **monotonically increasing** on $(a, b)$ if $a < x < y < b$ implies $f(x) \le f(y)$. If the last inequality is reversed, we obtain the definition of a **monotonically decrasing** function. The class ofmonotonic functions consists of both the increasing and the decreasing functions.


## Infinite Limits and Limits at Infinity


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

### 5.9 Theorem **Generalized Mean Value Theorem**
If $f$ and $g$ are continuous real functions on $[a, b]$ which are differentiable in $(a, b)$, then there is a point $x \in (a, b)$ at which

$[f(b)-f(a)]g'(x) = [g(b)-g(a)]f'(x)$.

Note that differntiability is not required at the endpoints.

**Proof:** Put

$h(t) = [f(b)-f(a)]g(t) - [g(b)-g(a)]f(t)$, $(a \le t \le b)$.

Then $h$ is continuous on $[a, b]$, $h$ is differentiable in $(a, b)$, and

$h(a) = f(b)g(a) - f(a)g(b) = h(b)$.

To prove the theorem, we have to show that $h'(x) = 0$ for some $x \in (a, b)$.

If $h$ is constant, this holds for every $x \in (a, b)$. If $h(t) > h(a)$ for some $t \in (a, b)$, let $x$ be a point on $[a, b]$ at which $h$ attains its maximum (Theorem 4.16). By $h(a) = f(b)g(a) - f(a)g(b) = h(b)$, and Theorem 5.8 shows that $h'(x) = 0$. If $h(t) < h(a)$ for some $t \in (a, b)$, the same argument applies if we choose for $x$ a point on $[a, b]$ where $h$ attains its minimum.

### 5.10 Theorem **Mean Value Theorem**
If $f$ is a real continuous function on $[a, b]$ which is differentiable in $(a, b)$, then there is a point $ x \in (a, b)$ at which

$f(b) - f(a) = (b - a)f'(x)$.



# 6 The Riemann-Stieltjes Integral


## Definition and Existence of the Integral

### 6.1 Definition
Let $[a, b]$ be a given interval. By a **partition** $P$ of $[a, b]$ we mean a finite set of points $x_0, x_1, \dots, x_n$, where
$$
a = x_0 \le x_1 \le \dots \le x_{n-1} \le x_n = b.
$$
We write
$$
\Delta x_i = x_i - x_{i-1}, (i = 1, \dots, n).
$$
Now suppose $f$ is a bounded real function defined on $[a, b]$. Corresponding to each partition $P$ of $[a, b]$ we put
$$
M_i = \sup f(x), (x_{i-1} \le x \le x_i),
$$
$$
m_i = \inf f(x), (x_{i-1} \le x \le x_i),
$$
$$
U(P, f) = \sum_{i=1}^n M_i \Delta_i,
$$
$$
L(P, f) = \sum_{i=1}^n m_i \Delta_i,
$$
and finally

**(Equation 6.1)** 
$$\overline{\int}_a^b f dx = \inf U(P, f),$$
**(Equation 6.2)**
$$
\underline{\int}_a^b f dx = \inf U(P, f),
$$
where the inf and the sup are taken over all partitions $P$ of $[a, b]$. The left members of (equation 6.1) and (equation 6.2) are called the **upper** and **lower Riemann integrals** of $f$ over $[a, b]$, respectively.

If the upper and lower integrals are equal, we say that $f$ is **Riemann integrable** on $[a, b]$, we write $f \in \mathscr{R}$ (that is, $\mathscr{R}$ denotes the set of Riemann-integrable functions), and we denote the common value of (equation 6.1) and (equation 6.2) by 
$$
\int_a^bfdx
$$ 
or 
$$
\int_a^bf(x)dx
$$
This is the Riemann integral of $f$ over $[a, b]$. Since $f$ is bounded, there exist two numbers, $m$ and $M$, such that
$$
m \le f(x) \le M, (a \le x \le b).
$$
Hence, for every $P$,
$$
m(b-a) \le L(P, f) \le U(P, f) \le M(b-a),
$$
so that the numbers $L(P, f)$ and $U(P, f)$ form a bounded set. This shows that **the upper and lower integrals are defined** for **every** bounded function $f$. The question of their equality, and hence the question of the integrability of $f$, is a more delicate one. Instead of investigating it separately for the Riemann integral, we shall immediately consider a more general situation.

### 6.2 Definition
Let $\alpha$ be a monotonically increasing function on $[a, b]$ (since $\alpha (a)$ and $\alpha (b)$ are finite, it follows that $\alpha$ is bounded on $[a, b]$). Corresbonding to each partition $P$ of $[a, b]$, we write
$$
\Delta\alpha_i = \alpha(x_i) - \alpha(x_{i-1})
$$
It is clear that $\Delta\alpha_i > 0$. For any real function $f$ which is bounded on $[a, b]$ we put
$$ U(P, f, \alpha) = \sum_{i=1}^nM_i\Delta\alpha_i $$
$$ L(P, f, \alpha) = \sum_{i=1}^nm_i\Delta\alpha_i $$
where $M_i$, $m_i$ have the same meaning as in Definition 6.1, and we define
**(Equation 6.5)** 
$$\overline{\int}_a^b f d\alpha = \inf U(P, f, \alpha),$$
**(Equation 6.6)** 
$$\underline{\int}_a^b f d\alpha = \sup L(P, f, \alpha),$$
the $\inf$ and $\sup$ again being taken over all partitions.

If the left members of (equation 6.5) and (equation 6.6) are equal, we denote their common value by

**(Equation 6.7)** 
$$ \int_a^bd\alpha $$
or sometimes by

**(Equation 6.8)** 
$$ \int_a^bd\alpha(x) $$

This is the *Riemann-Stieltjes* integral (or simply the **Stieljes integral**) of $f$ with respect to $\alpha$, over $[a, b]$.

If (equation 6.7) exists, i.e, if (equation 6.5) and (equation 6.6) are equal, we say that $f$ is integrable with respect to $\alpha$, in the Riemann sense, and write $f \in \mathscr{R}(\alpha)$.

By taking $\alpha(x) = x$, the Riemann integral is seen to be a special case of the Riemann-Stieltjes integral. Let us mention explicitly, however, that in the general case $\alpha$ need not even be continuous.

### 6.3 Definition
We say that the partition $P^*$ is a refinement of $P$ if $P^* \supset P$ (that is, if every point of $P$ is point of $P^*$). Given two partitions, $P_1$ and $P_2$, we say that $P^*$ is their common refinement if $P^* = P_1 \cup P_2$.

### 6.4 Theorem
If $P^*$ is a refinement of $P$, then
$$ L(P, f, \alpha) \le L(P^*, f, \alpha) $$
and
$$ U(P^*, f, \alpha) \le U(P, f, \alpha) $$

### 6.5 Theorem
$$ \underline{\int}_a^bfd\alpha \le \overline{\int}_a^bfd\alpha $$

### 6.6 Theorem
$f \in \mathscr{R}(\alpha)$ on $[a, b]$ if and only if for every $\epsilon > 0$ there exists a partition $P$ such that
**(equation 6.13)**
$$ U(P, f, \alpha) - L(P, f, \alpha) < \epsilon $$


### 6.7 Theorem
1. If (equation 6.13) holds for some $P$ and some $\epsilon$, then (equation 6.13) holds (with the same $\epsilon$) for every refinement of $P$.
2. If (equation 6.13) holds for $P = \{x_0, \dots, x_n\}$ and if $s_i$, $t_i$ are arbitrary points in $[x_{i-1}, x_i]$, then
   $$ \sum_{i=1}^n \left|f(s_i)-f(t_i)\right|\Delta\alpha_i < \epsilon $$
3. If $f \in \mathscr{R}(\alpha)$ and the hypotheses of 2. hold, then
   $$ \left|\sum_{i=1}^nf(t_i)\Delta\alpha_i-\int_a^bfd\alpha\right| < \epsilon $$

### 6.8 Theorem
If $f$ is continuous on $[a, b]$ then $f \in \mathscr{R}(\alpha)$ on $[a, b]$.

### 6.9 Theorem
If $f$ is monotonic on $[a, b]$, and if $\alpha$ is continuous on $[a, b]$, then $f \in \mathscr{R}(\alpha)$. (We still assume, of course, that $\alpha$ is monotonic.)

### 6.10 Theorem
Suppose $f$ is bounded on $[a, b]$, $f$ has only finitely many points of discontinuity on $[a, b]$, and $\alpha$ is continuous at every point at which $f$ is discontinuous. Then $f \in \mathscr{R}(\alpha)$.

### 6.11 Theorem
Suppose $f \in \mathscr{R}(\alpha)$ on $[a, b]$, $m \le f \le M$, $\phi$ is continuous on $[m, M]$, and $h(x) = \phi(f(x))$ on $[a, b]$. Then $h \in \mathscr{R}(\alpha)$ on $[a, b]$.


## Properties of The Integral

### 6.12 Theorem
1. If $f_1 \in \mathscr{R}(\alpha)$ and $f_2 \in \mathscr{R}(\alpha)$ on $[a, b]$, then
    $$ f_1 + f_2 \in \mathscr{R}(\alpha) $$
    $cf \in \mathscr{R}(\alpha)$ for every constant $c$, and
    $$\int_a^b(f_1+f_2)d\alpha = \int_a^bf_1d\alpha + \int_a^bf_2d\alpha$$
    $$\int_a^bcf d\alpha = c\int_a^bf d\alpha$$
2. If $f_1(x) \le f_2(x)$ on $[a, b]$, then
    $$\int_a^bf_1d\alpha \le \int_a^bf_2d\alpha$$
3. If $f \in \mathscr{R}(\alpha)$ on $[a, b]$ and if $a < c < b$, then $f \in \mathscr{R}(\alpha)$ on $[a, c]$ and on $[c, b]$, and
    $$\int_a^cfd\alpha + \int_c^bfd\alpha = \int_a^bfd\alpha$$
4. If $f \in \mathscr{R}(\alpha)$ on $[a, b]$ and if $|f(x)| \le M$ on $[a, b]$, then
    $$\left|\int_a^bfd\alpha\right| \le M[\alpha(b) - \alpha(a)]$$
5. If $f \in \mathscr{R}(\alpha_1)$ and $f \in \mathscr{R}(\alpha_2)$, then $f \in \mathscr{R}(\alpha_1+\alpha_2)$ and
    $$\int_a^bfd(\alpha_1+\alpha_2) = \int_a^bfd\alpha_1 + \int_a^bfd\alpha_2$$
    if $f \in \mathscr{R}(\alpha)$ and $c$ is a positive constant, then $f \in \mathscr{R}(c\alpha)$ and
    $$\int_a^bfd(c\alpha) = c\int_a^bfd\alpha$$

### 6.13 Theorem
If $f \in \mathscr{R}(\alpha)$ and $g \in \mathscr{R}(\alpha)$ on $[a, b]$, then
1. $fg \in \mathscr{R}$;
2. $|f| \in \mathscr{R}(\alpha)$ and $\left|\int_a^bfd\alpha\right| \le \int_a^b|f|d\alpha$.

### 6.14 Definition
The unit step function $I$ is defined by
$$I(x) = \begin{cases}0\hspace{10pt}(x \le 0),\\1\hspace{10pt}(x > 0).\end{cases}$$

### 6.15 Theorem
If $a < s < b$, is bounded on $[a, b]$, $f$ is continuous at $s$, and $\alpha(x) = I(x-s)$, then
$$\int_a^bfd\alpha=f(s).$$

### 6.16 Theorem
Suppose $c_n \ge 0$ for $1, 2, 3, \dots$, $\sum c_n$ converges, $\{s_n\}$ is a sequence of distinct points in $(a, b)$, and
$$\alpha(x) = \sum_{n=1}^\infty c_nI(x-s_n).$$
Let $f$ be continuous on $[a, b]$. Then
$$\int_a^bfd\alpha = \sum_{n=1}^\infty c_nf(s_n).$$



# 7 Sequences and Series of Functions


## Discussion of Main Problem

### 7.1 Definition
Suppose $\{f_n\}, n = 1, 2, 3, \dots,$ is asequence of functions defined on a set $E$, and suppose that the sequence of numbers $\{f_n(x)\}$ converges for every $x \in E$. We can then define a function $f$ by

**(eqution 7.1)** $f(x) = \lim\limits_{n \to \infty} f_n(x), (x \in E)$.

Under these circumstances we say that $\{f_n\}$ converges on $E$ and that $f$ is the **limit**, or the **limit function**, of $\{f_n\}$. Sometimes we shall use a more descriptive terminology and shall say that "$\{f_n\}$ converges to $f$ **pointwise** on $E$" if (equation 7.1) holds. Similarly, if $\sum f_n(x)$ converges for every $x \in E$, and if we define

**(equation 7.2)** $f(x) = \sum\limits_{n=1}^\infty f_n(x), (x \in E)$,

the function $f$ is called the **sum** of the series $\sum f$.


# 8 Some Special Functions


## The Exponential and Logarithmic Functions

We define

**(equation 1)** $E(z) = \sum\limits_{n=0}^\infty \frac {z^n} {n!}$

The ratio test shows that this series converges for every complex $z$.


## The Trigonometric Functions

Let us define

$C(x) = \frac 1 2 [E(ix)+E(ix)]$, 


## Fourier Series


### 8.9 Definition
A **trigonometric polynomial** is a finite sum of the form

$f(x) = a_0 + \sum\limits_{n=1}^N(a_n\cos nx + b_n\sin nx)$ (x real),

where $a_0,...,a_N,b_1,...,b_N$ are complex numbers. On account of the identities





# 11 The Lebesgue Theory

## Measure Spaces


### 11.12 Definition
Suppose $X$ is a set, not necessarily a subset of a euclidean space, or indeed of any metric space. $X$ is said to be a **measure space** if there exists a $\sigma$-ring $\mathfrak{M}$ of subsets of $X$ (which are called measurable sets) and a non-negative countably additive set function $\mu$ (which is called a measure), defined on $\mathfrak{M}$.