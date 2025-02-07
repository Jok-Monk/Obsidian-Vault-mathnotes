

> [!PDF|important] [[Real Analysis - 2nd Edition (Gerald B. Folland) (.pdf#page=44&selection=0,16,1,1&color=important|p.44]]
> > 1.7 Proposition. If ε is an [[elementary family]], the collection of finite disjoint unions of members of ε is an [[algebra]]
> 

>[!Prove]- Prove:
>设$\mathcal{A}$为$\varepsilon$中的有限不交并，$\mathcal{A}$明显非空。$\forall A_{j}\text{有限不交}\in \mathcal{A}$，往证$\bigcup_{j}A_{j}\in \mathcal{A}$，只需证$\forall \{ A_{j} \}_{j=1}^{n}\subset\varepsilon,\cup A_{j}\in \mathcal{A}$
>$A,B\in\varepsilon,B^{c}=\bigcup_{1}^{J}C_{j},C_{j}\in\varepsilon\ disjoint\implies A\setminus B=A\cap(\cup C_{j})=\cup(A\cap C_{j})\text{为不交并}\in \mathcal{A}$
>$A\cup B=(A\setminus B)\cup B\in \mathcal{A}$
>假设$J=n-1$时成立，
>$J=n$时，由归纳假设，可设$\bigcup_{j=1}^{n-1}A_{j}=\bigcup_{j=1}^{m}B_{j}$为$\varepsilon$中的不交并
>$\bigcup_{j=1}^{n}A_{j}=A_{n}\cup(\bigcup_{j=1}^{m}B_{j}\setminus A_{n})$为$\varepsilon$中的不交并，于是$\bigcup_{j=1}^{n}A_{j}\in \mathcal{A}$
>现在证明$\mathcal{A}$对补集封闭
>设$A_{1},\dots A_{n}\in \varepsilon$是不交的，$A_{m}^{c}=\bigcup_{j=1}^{J_{m}}B_{m}^{j}$，其中$\{ B_{m}^{j} \}_{j=1}^{J_{m}}$是$\varepsilon$中的不交集
>$\left( \bigcup_{m=1}^{n}A_{m} \right)^{c}=\left( \bigcup_{m=1}^{n}\left( \bigcup_{j=1}^{J_{m}}B_{m}^{j} \right)^{c} \right)^{c}=\bigcap_{m=1}^{n}\left( \bigcup_{j=1}^{J_{m}}B_{m}^{j} \right)=\bigcup \{ \cap_{i=1}^{n}B_{i}^{j_{i}}:1\leq j_{m}\leq J_{m},1\leq m\leq n \}$是不交并，因此$\in \mathcal{A}$
>
>



