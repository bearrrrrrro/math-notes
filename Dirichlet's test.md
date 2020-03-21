## Dirichlet's test

Assume $S_n = \sum_{k=1}^n a_k$ is a bounded sequence and $b_n$ dec. to 0. Then $\sum a_n b_n$ conv.

## Abel's test

Assume that $\sum a_n$ conv. and $\{b_n\}$ is monotonically convergent sequence. Then $\sum a_n b_n$ conv.

pf. From $\sum_{k=1}^n a_kb_k = A_nb_{n+1} - \sum_{k=1}^nA_k(b_{k+1}-b_k)$ for Dirichlet's test, 

$\lim_{n \to \infty} A_nb_{n+1} = 0$

$$|\sum_{k=1}^n A_k(b_{k+1}-b_k)| \leq \sum_{k=1}^n|A_k|(b_k - b_{k+1}) \leq M\sum_{k=1}^n(b_k-b_{k+1})$$



For Abel's test, $\lim_{n \to \infty} A_nb_{n+1}$ exists.

Now $\sum a_k$ conv $\Rightarrow$ $|A_n| \leq M \forall n$ 

Question: $\sum_{n=1}^\infty \frac{e^{inx}}{n} \forall x \in \R$ conv.?

Check $(1-e^{ix})\sum_{k=1}^n e^{ikx} = \sum_{k=1}^n[e^{ikx}-e^{i(k+1)x}]=e^{ix}-e^{i(n+1)x}$

$\sum_{k=1}^ne^{ikx}=\frac{e^{ix}-e^{i(n+1)x}}{1-e^{ix}} = \frac{e^{ix}-e^{inx/2}(e^{inx/2}-e^{-inx/2})}{e^{ix/2}(e^{ix/2}-e^{-ix/2})} = \frac{e^{inx/2}-e^{-inx/2}}{e^{ix/2}-e^{-ix/2}}e^{i(n+1)x/2}=\frac{sin(nx/2)}{sin(x/2)}e^{i(n+1)x/2}$

So $|\sum_{k=1}^ne^{ikx}|\leq\frac{1}{|sim(x/2)}\Rightarrow |\sum_{k=1}^ne^{ikx}|$ is bounded if $x \neq  2m\pi, m \in \Z$.

By Dirichlet's test, $\sum_{n=1}^\infty\frac{e^{inx}}{n}$ conv. if $x\neq 2m\pi$.

## Rearrangement of a series

Let $f:\Z_+\to\Z_+$ onto and 1-1

Define the series $\sum b_n=\sum a_{f(n)}$

Theorem. If $\sum a_n$ converges abs., then $\sum b_n$ conv. abs. If $\sum a_n$ conv. abs. and $\sum a_n=S$, then $\sum b_n = S$

pf. 1. Assume that $\sum a_n$ conv. abs, i.e. $\sum |a_n|$ conv.

Let $S_n = \sum_{k=1}^n a_k, t_n = \sum_{k=1}^n b_k$, then 

$|t_n|=|\sum_{k=1}^n b_k| \leq \sum_{k=1}^n |b_k| = \sum_{k=1}^n |a_{f(k)}| \leq \sum_{k=1}^{\max\{f(1), …, f(n)\}}|a_k| < \infty$

$\Rightarrow \sum |b_n|$ conv.

2. Assume $\sum a_n = S$, i.e. $S_n \to S$ .

   $\forall \epsilon > 0, \exists N=N(\epsilon)>0$ s.t. $|S_N-S|$ and $\sum_{k=1}^\infty |a_{N+k}|<\epsilon/2$

   $|t_n-S|\leq |t_n-S_n|+|S_N-S|<\epsilon/2$

   We can find $M>0$ s.t. $\{1, 2, …, N\}\subset\{f(1), …, f(M)\}$. So if $n>M$, then $f(n)>N$. Hence for $n>M$, 

 