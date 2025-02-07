> [!PDF|important] [[Real Analysis - 2nd Edition (Gerald B. Folland) (.pdf#page=78&selection=21,0,21,12&color=important|p.78]]
> > 2.15 Theorem $\{ f_{n} \}$是$L^{+}$中的有限或可数无穷序列，$f=\sum_{n}f_{n}$，那么
> > $\int f=\sum_{n}\int f_{n}$

>[!Prove]- 
> 有限情形只需考虑$n=2$的情况
> 设$f_{1},f_{2}\in L^{+},\{ \phi_{j} \},\{ \psi_{j} \}$分别是单调递增逐点趋于$f_{1},f_{2}$的简单函数，那么$\{ \phi_{j}+\psi_{j} \}$为单调递增逐点趋于$f_{1}+f_{2}$的简单函数·，由[[monotone convergence theorem]]和[[theorem 2.13]]b有
> $\int(f_{1}+f_{2})=\lim_{ j \to \infty }\int(\phi_{j}+\psi_{j})=\lim_{ j \to \infty }\int\phi_{j}+\lim_{ j \to \infty }\int \psi_{j}=\int f_{1}+\int f_{2}$
> 归纳可得$\int \sum_{1}^{N}f_{n}=\sum_{1}^{N}\int f_{n}$
> 令$N\to \infty$，应用[[monotone convergence theorem]]可得$\int\sum_{n=1}^{\infty}f_{n}=\lim_{ N \to \infty }\int \sum_{n=1}^{N}f_{n}=\lim_{ N \to \infty }\sum_{n=1}^{N}\int f_{n}=\sum_{n=1}^{\infty}\int f_{n}$
> $\Box$