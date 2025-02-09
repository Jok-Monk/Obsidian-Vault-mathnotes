![[Real Analysis - 2nd Edition (Gerald B. Folland) (.pdf#page=50&rect=75,336,542,442&color=important|Real Analysis - 2nd Edition (Gerald B. Folland) (, p.50]]
>[!Prove]- 
>1. $0\leq\mu^{*}(\emptyset)\leq \sum \rho(\emptyset)=0\implies \mu^{*}(\emptyset)=0$
>2. $A\subset B\implies \left( \forall \{ E_{j} \}\subset\varepsilon:B\subset\bigcup E_{j}\implies A\subset\bigcup E_{j} \right)$$\implies \forall \{ E_{j} \}:B\subset\bigcup E_{j},\mu^{*}(A)\leq \sum \rho(E_{j})\implies \mu^{*}(A)\leq \mu^{*}(B)$
>3. $A:=\bigcup A_{j},A_{j}\in\varepsilon,\forall \epsilon,\forall j,\exists \{ E_{j}^{i} \}:A_{j}\subset \bigcup_{i}E_{j}^{i},\mu^{*}(A_{j})>\sum_{i}\rho(E_{j}^{i})-\epsilon 2^{-j},\sum_{j}\mu^{*}(A_{j})\geq \sum_{i,j}\rho(E_{j}^{i})-\epsilon\geq \mu^{*}(A)-\epsilon$对任意$\epsilon$成立，于是$\mu^{*}(A)\geq \sum_{j}\mu^{*}(A_{j})$
