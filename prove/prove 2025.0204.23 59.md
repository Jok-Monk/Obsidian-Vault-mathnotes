>[!prove]
>$\mathcal{X}_{A}(x)\mathcal{X}_{B}(y)=1\Leftrightarrow\mathcal{X}_{A}(x)=1\ and\ \mathcal{X}_{B}(y)=1\Leftrightarrow x\in A\ and\ y\in B\Leftrightarrow (x,y)\in A\times B\Leftrightarrow \mathcal{X}_{A\times B}(x,y)=1$
>于是$\mathcal{X}_{A}(x)\mathcal{X}_{B}(y)=\mathcal{X}_{A\times B}(x,y)$
>$(x,y)\in A\times B=\bigcup_{j}A_{j}\times B_{j}$是不交的，$\Leftrightarrow \exists j,(x,y)\in A_{j}\times B_{j},\forall i\neq j,(x,y)\not\in A_{i}\times B_{i}$
>于是$\mathcal{X}_{A\times B}(x,y)=\sum_{j}\mathcal{X}_{A_{j}\times B_{j}}(x,y)$
>同理有$\mathcal{X}_{A_{j}\times B_{j}}(x,y)=\mathcal{X}_{A_{j}}(x)\mathcal{X}_{B_{j}}(y)$
>$\sum_{j}\mathcal{X}_{A_{j}\times B_{j}}(x,y)=\sum_{j}\mathcal{X}_{A_{j}}(x)\mathcal{X}_{B_{j}}(y)$
>$\Box$
