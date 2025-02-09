>[!prove]
>* $\emptyset=\emptyset \times \emptyset,\pi(\emptyset)=\pi(\emptyset \times \emptyset)=\mu(\emptyset)\nu(\emptyset)=0\times 0=0$
>* 设$\{ E_{j} \}_{j=1}^{\infty}\subset \mathcal{A}$为一列不交集，且$\bigcup_{j=1}^{\infty}E_{j}\in \mathcal{A}$
>设$E=\bigcup_{j=1}^{\infty}E_{j}=\bigcup_{r=1}^{n}A_{r}\times B_{r}$为不交并$E_{j}=\bigcup_{i=1}^{n_{j}}A_{j}^{i}\times B_{j}^{i}$为不交并，$A_{r}\times B_{r}=(A_{r}\times B_{r})\cap E=(A_{r}\times B_{r})\cap\left( \bigcup_{j=1}^{\infty}\bigcup_{i=1}^{n_{j}}A_{j}^{i}\times B_{j}^{i} \right)=\bigcup_{j=1}^{\infty}\bigcup_{i=1}^{n_{j}}((A_{r}\cap A_{j}^{i})\times(B_{r}\cap B_{j}^{i}))$
>$E_{j}=\bigcup_{i=1}^{n_{j}}A_{j}^{i}\times B_{j}^{i}=\left( \bigcup_{i=1}^{n_{j}}A_{j}^{i}\times B_{j}^{i} \right)\cap\left( \bigcup_{r=1}^{n}A_{r}\times B_{r} \right)=\bigcup_{i=1}^{n_{j}}\bigcup_{r=1}^{n}((A_{j}^{i}\cap A_{r})\times(B_{j}^{i}\cap B_{r}))$
>$\pi(E)=\sum_{r=1}^{n}\mu(A_{r})\nu(B_{r})=\sum_{r=1}^{n}\sum_{j=1}^{\infty}\sum_{i=1}^{n_{j}}\mu(A_{j}\cap A_{r})\nu(B_{j}^{i}\cap B_{r})=\sum_{j=1}^{\infty}\sum_{i=1}^{n_{j}}\sum_{r=1}^{n}\mu(A_{j}^{i}\cap A_{r})\nu(B_{j}^{i}\cap B_{r})=\sum_{j=1}^{\infty}\pi(E_{j})$
>$\Box$
