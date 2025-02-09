![[Real Analysis - 2nd Edition (Gerald B. Folland) (.pdf#page=51&rect=72,384,543,450&color=important|Real Analysis - 2nd Edition (Gerald B. Folland) (, p.51]]
[[sigma-algebra]]
>[!Prove]- 
>- $A\in \mathcal{M}\implies \mu^{*}(E)=\mu^{*}(E\cap A)+\mu^{*}(E\cap A^{c}),\forall E\in \mathcal{M}$  $\implies A^{c}\in \mathcal{M}$
>$\implies A^{c}\in \mathcal{M}$
>- 设$A,B\in \mathcal{M},\mu^{*}(E)\leq \mu^{*}(E\cap(A\cup B))+\mu^{*}(E\cap(A\cup B)^{c})$
>$\leq \mu^{*}(E\cap A\cap B)+\mu^{*}(E\cap A^{c}\cap B)+\mu^{*}(E\cap A\cap B^{c})+\mu^{*}(E\cap A^{c}\cap B^{c})$
>$=\mu^{*}(E\cap B)+\mu^{*}(E\cap B^{c})$
>$=\mu^{*}(E),\forall E\in \mathcal{P}(X)$
>于是$A\cup B\in \mathcal{M}$
>且$A\cap B=\emptyset\implies \mu^{*}(A\cup B)=\mu^{*}((A\cup B)\cap A)+\mu^{*}((A\cup B)\cap A^{c})=\mu^{*}(A)+\mu^{*}(B)$，即$\mu^{*}$是有限可加的
>对于一列不交的$\{ A_{j} \}_{1}^{\infty}\subset \mathcal{M},$记$B=\bigcup_{1}^{\infty}A_{j},B_{n}=\bigcup_{1}^{n}A_{j}$
>$\mu^{*}(E\cap B_{n})=\mu^{*}(E\cap B_{n}\cap A_{n})+\mu^{*}(E\cap B_{n}\cap A_{n}^{c})=\mu^{*}(E\cap A_{n})+\mu^{*}(E\cap B_{n-1})$
>>错误证法：$\mu^{*}(E\cap B_{n})=\mu^{*}(E\cap B_{n-1})+\mu^{*}(E\cap A_{n})$，
>>$E\cap A_{n}$和$E\cap B_{n-1}$不一定属于$\mathcal{M}$，不能直接使用有限可加性
>>
>- $\forall n,\mu^{*}(E)=\mu^{*}(E\cap B_{n})+\mu^{*}(E\cap B_{n}^{c})$  
>$\geq \mu^{*}(E\cap B_{n})+\mu^{*}(E\cap B^{c})$
>$=\sum_{i=1}^{n}\mu^{*}(E\cap A_{i})+\mu^{*}(E\cap B^{c})$
>$n\to \infty,\mu^{*}(E)\geq \sum_{i=1}^{\infty}\mu^{*}(E\cap A_{i})+\mu^{*}(E\cap B^{c})$
>$\geq \mu^{*}(E\cap B)+\mu^{*}(E\cap B^{c})$
>从而$B=\bigcup_{1}^{\infty}A_{j}\in \mathcal{M}$
>取$E=B$，有$\mu^{*}(B)=\sum_{i=1}^{\infty}\mu^{*}(A_{i})$
>于是$\mathcal{M}$确实为$\sigma$-代数，且$\mu^{*}_{|\mathcal{M}}(\emptyset)=\mu^{*}(\emptyset)=0$
>即$\mu^{*}_{|\mathcal{M}}$为·$\mathcal{M}$上的测度
>$N\in \mathcal{M},\mu^{*}(N)=0\implies \forall A\subset N,\mu^{*}(E)\leq\mu^{*}(E\cap A)+\mu^{*}(E\cap A^{c})\leq \mu^{*}(N)+\mu^{*}(E)=\mu^{*}(E)$
>从而$A\in \mathcal{M}$该测度是完备的

