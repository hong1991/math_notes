# Week 1

**Definition.** A *vector space* is any collection $V$ of objects (called *vectors*) for which two operations can be performed:

- *Vector addition*, whichtakes two vectors $v$ and $w$ in $V$ and returns another vector $v+w$ in $V$. (Thus $V$ must be closed under addition).

- *Scalar multiplication*, which takes a scalar $c$ in $\mathbf{R}$ and a vector $v$ in $V$, and returns another vector $cv$ in $V$. (Thus $V$ must be closed under scalar multiplication).

Futhermore, for *V* to be a vector space, the following properties must be satisfied:

1. (Addtion is commutative) For all $v, w \in V$, $v+w=w+v$.

2. (Addition is associative) For all $u, v, w \in V$, $u+(v+w)=(u+v)+w$.

3. (Additive identity) There is a vector $0 \in V$, called the *zero vector*, such that $0+v=v$.

4. (Additive inverse) For each vector $v \in V$, there is a vector $-v \in V$, called the *addtive inverse* of $v$, such that $-v+v=0$.

5. (Multiplicative identity) The scalar $1$ has the property that $1v = v$ for all $v \in V$.

6. (Multiplication is assosiative) For any scalars $a, b \in \mathbf{R}$ and any vector $v \in V$, we have $a(bv)=(ab)v$.

7. (Muliplication is linear) For any scalar $a \in \mathbf{R}$ and any vectors $v, w \in V$, we have $a(v+w)=av+aw$.

8. (Muliplication distributes over addtition) For any scalars $a, b \in \mathbf{R}$ and any vector $v \in V$, we have $(a+b)v=av+bv$.

> We never say exactly what vectors *are*, only what vectors *do*. This is an example of *abstraction*, which appears everywhere in mathematics (but especially in algebra): the exact substance of an object is not important, only its properties and functions.

---

**Vector cancellation law** If $u, v, w$ are vectors such that $u+v=u+w$, then $v=w$.

> **Proof:** Since $u$ is a vector, we have an additive inverse $-u$ such that $-u+u=0$, by axiom 4. Now we add $-u$ to both sides of $u+v=v+u$:
>
> $$-u+(u+v)=-u+(u+w).$$
>
> Now use axiom 2:
>
> $$(-u+u)+v=(-u+u)+w$$
>
> then axiom 4:
>
> $$0+v=0+w$$
>
> then axiom 3:
>
> $$v=w.$$

---

**Vector subspaces** A vector space $W$ is a subspace of a vector space $V$ if $W \subseteq V$, and the laws of vector addition and scalar multiplication are consistent.

**Lemma.** Let $V$ be a vector space, and let $W$ be a subset of $V$. Then $W$ is a subspace of $V$ if and only if the following two properties are satisfied:

* ($W$ is closed under addition) If $w_{1}$ and $w_{2}$ are in $W$, then $w_{1}+w_{2}$ is also in $W$.

* ($W$ is closed under scalar multiplication) If $w$ is in $W$ and $c$ is a scalar, then $cw$ is also in $W$.

> **Proof:** First suppose that $W$ is a subspace of $V$. Then $W$ will be closed under addition and multiplication directly from the definition of vector space. This proves the "only if" part.
>
> Now we prove the harder "if part". In other words, we assume that $W$ is a subset of $V$ which is closed under addition and scalar multiplication, and we have to prove that $W$ is a vector space.  In other words, we have to verify the axioms 1-8.
>
> Most of these axioms follow immediately because $W$ is a subset of $V$, and $V$ already obeys the axioms 1-8. For instance, since vectors $v_{1}$, $v_{2}$ in $V$ obey the commutativity property $v_{1}+v_{2}=v_{2}+v_{1}$, it automatically follows that vectors in $W$ also obey the property $w_{1}+w_{2}=w_{2}+w_{1}$, since all vectors in $W$ are also vectors in $V$. This reasoning easily gives us axioms 1, 2, 5, 6, 7, 8.
>
> There is a potential problem with 3 though, because the zero vector $0$ of $V$ might not lie in $W$. Similarly with 4, there is a potential problem that if $w$ lies in $W$, then $-w$ might not lie in $W$. But both problems cannot occur, because $0=0w$ and $-w=(-1)w$, and $W$ is closed under scalar multiplication.

# Week 2