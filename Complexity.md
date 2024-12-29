## Some theorems

### thm1

Let $f$ be an increasing function that satisfies the recurrance relation:
$$f(n)=af(n/b)+c$$
whenever $n$ is devisible by $b$, $a\geq 1, b\in N\gt 1$, $c$ is a positive real number, then:
$$
f(n)=
\begin{cases}
O(n^{\log^a_b}), \text{if }a>1\\
O(\log{n}), \text{if }a=1
\end{cases}
$$
Furthermore, when $n=b^k$ and $a\neq 1$, where $k$ is a positive number,
$$f(n)=C_1n^{\log^a_b}+C_2$$
where $C_1=f(1)+c/(a-1)$ and $C_2 = -c/(a-c)$







