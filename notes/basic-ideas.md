# Topological Spaces

### Definition. Topological Spaces

Let $X$ be any set.

A family $\mathcal T \subseteq \mathcal P(X)$ is a **topology** on $X$ iff it satisfies the **open set axioms** as following.

1. $X \in \mathcal T$.

2. $\mathcal T$ is closed under arbitrary union. That is, for any $\mathcal U \subseteq \mathcal T$, $\bigcup \mathcal U \in \mathcal T$.
3. $\mathcal T$ is closed under finite intersection. That is, for any finite $\mathcal U \subseteq \mathcal T$, $\bigcap \mathcal U \in \mathcal T$.

The ordered pair $(X, \mathcal T)$ is a **topological space** iff $\mathcal T$ is a topology on $X$.

A subset $U \subseteq X$ is an **open set** of $(X, \mathcal T)$, or **open subset** of $X$ (with the topology $\mathcal T$), iff $U \in \mathcal T$.

### Note. A Topology Is Not Necessarily Closed Under Infinite Intersection

Some topologies are closed under arbitrary intersection, e.g., the discrete topologies, but some are not. For example, let $\mathcal T$ be a Euclidean topology on $\mathbb R$, then all intervals in $\mathbb R$ is open in $(X, \mathcal T)$. But
$$
\bigcap \left\{ \left( -\frac{1}{n}, \frac{1}{n} \right) \right\}_{n \in \mathbb Z_{> 0}} = \{0\},
$$
which is not open in $(X, \mathcal T)$.

### Lemma. Empty Set Is an Element of Any Topologies

Let $(X, \mathcal T)$ be a topological space.

Then $\emptyset \in \mathcal T$.

**Proof.** $\emptyset$ is the subset of any set, so $\emptyset \subseteq \mathcal T$. Then, we have
$$
\emptyset = \bigcup \emptyset \in \mathcal T.
$$
$\blacksquare$

### Example. Euclidean Topologies for $\mathbb R^n$

In $\mathbb R^n$, we define a mapping $\rho: X \times X \to \mathbb R_{\ge 0}$ as
$$
\rho(\mathbf x, \mathbf y) := \left( \sum_{i = 1}^n |x_i - y_i|^2 \right)^\frac{1}{2}.
$$
For any $\mathbf x \in \mathbb R^n$ and for any $\delta \in \mathbb R_{> 0}$, we define
$$
B(\mathbf x, \delta) := \left\{ \mathbf y \in \mathbb R^n : \rho(\mathbf x, \mathbf y) < \delta \right\}.
$$
Let
$$
\mathcal T := \bigcup\left\{ B(\mathbf x, \delta) : \mathbf x \in \mathbb R^n \land \delta \in \mathbb R_{> 0} \right\}.
$$
Then, $\mathcal T$ is a topology for $\mathbb R^n$, called **Euclidean topology**.

### Definition. Comparations of Topologies

Let $X$ be any set, and let $\mathcal T_1$ and $\mathcal T_2$ be topologies for $X$.

$\mathcal T_1$ is **coarser** than $\mathcal T_2$, or $\mathcal T_2$ is **finer** than $\mathcal T_1$, iff $\mathcal T_1 \subseteq \mathcal T_2$.

### Example. Discrete Topologies

For any set $X$, its power set $\mathcal P(X)$ is the **discrete topology** for $X$. It is the finest topology for $X$.

### Example. Indiscrete Topologies

For any set $X$, the collection $\{\emptyset, X\}$ is the **indiscrete topology**, or **trivial topology**, for $X$. It is the coarsest topology for $X$.















