
> [!PDF|note] [[Real Analysis - 2nd Edition (Gerald B. Folland) (.pdf#page=95&selection=107,0,107,20&color=note|p.95]]
> > 2.5 PRODUCT MEASURES

设$(X,\mathcal{M},\mu),(X,\mathcal{N},\nu)$为测度空间
我们已经讨论过$X\times Y$上的$\sigma$-代数$\mathcal{M}\otimes \mathcal{N}$ [[product sigma algebra]] ，现在我们尝试构建其上的测度$\mu \times \nu$ 
>[!definition] 
>>(measurable) rectangle form $A\times B$,$A\in \mathcal{M},B\in \mathcal{N}$,

由于$(A\times B)\cap(E\times F)=(A\cap E)\times(B\cap F)$      ,    $(A\times B)^c=(X\times B^c)\cup(A^c\times B)$ 
由[[Proposition 1.7]] 知，所有rectangle的有限不交并组成的集族$\mathcal{A}$构成一个代数，其生成的$\sigma$-代数自然是$\mathcal{M}\otimes \mathcal{N}$[[prove 2025.0204.23 35]]
设rectangle$A\times B$是一些(可数或有限)个rectangle$A_{j}\times B_{j}$的不交并，则对于$x\in X, y\in Y$，
$\mathcal{X}_{A}(x)\mathcal{X}_{B}(y)=\mathcal{X}_{A\times B}(x,y)=\sum \mathcal{X}_{A_{j}\times B_{j}}(x,y)=\sum \mathcal{X}_{A_{j}}(x)\mathcal{X}_{B_{j}}(y)$[[prove 2025.0204.23 59]]
如果我们对$x$积分，由[[theorem 2.15]]知，
$\mu(A)\mathcal{X}_{B}(y)=\int \mathcal{X_{A}}(x)\mathcal{X}_{B}(y)d\mu(x)=\sum \int \mathcal{X}_{A_{j}}(x)\mathcal{X}_{B_{j}}(y)d\mu(x)=\sum \mu(A_{j})\mathcal{X}_{B_{j}}(y)$[[prove 2025.0205.00 05]]
同理，对$y$积分，有
$\mu(A)\nu(B)=\sum \mu(A_{j})\nu(B_{j})$
这说明了对于$E\in \mathcal{A},E=A_{1}\times B_{1},\dots A_{n}\times B_{n}$的不交并
$\pi(E):=\\\sum_{j=1}^{n}\mu(A_{j})\nu(B_{j})$
是$\mathcal{A}$上良定义的[[prove 2025.0205.00 15]]
由[[Theorem 1.14]]，$\pi$是$\mathcal{A}$上的[[预测度]],[[prove 2025.02.09.15 25]]于是$\pi$生成了$X\times Y$上的外测度，其在$\mathcal{M}\otimes \mathcal{N}$上的限制称为$\mu$与$\nu$的乘积测度，记作
>[!Definition]
>>$\mu \times \nu$

若$\mu,\nu$均为$\sigma$-有限的，则$\mu \times \nu$也是$\sigma$-有限的[[prove 2025.0205.00 26]]
此时，由[[Theorem 1.14]],$\mu \times \nu$是$\mathcal{M}\otimes \mathcal{N}$上唯一满足$(\mu \times \nu)(A\times B)=\mu(A)\nu(B)$对所有rectangle$A\times B$成立的测度
若$\mu,\nu$均为完全的$\implies\,\mu \times \nu$是完全的？[[draft]]
对有限个测度空间$(X_{j},\mathcal{M}_{j},\mu_{j})$，可以递归定义$\mu_{1}\times\dots \times\mu_{n}$
>[!Definition]
>>$\mu_{1}\times\dots \times \mu_{n}=(\mu_{1}\times\dots \times \mu_{n-1})\times \mu_{n}$

定义$X_{1}\times\dots X_{n}$上的rectangle为：$A_{1}\times\dots \times A_{n},with A_{j}\in \mathcal{M}_{j}$
同样可以验证所有矩形的有限不交并构成一个代数
定义$(\mu_{1}\times\dots \times\mu_{n})(A_{1}\times\dots \times A_{n})=\prod_{j=1}^{n}\mu_{j}(A_{j}),with A_{j}\in \mathcal{M}_{j}$
同样可以验证其诱导了$\mathcal{M}_{1}\otimes\dots \otimes \mathcal{M}_{n}$上的测度$(\mu_{1}\times\dots \times \mu_{n})$
>[!Definition]
>>$(\mu_{1}\times\dots \times \mu_{n})$

可以验证这两种定义是等价的？[[draft]]

现在我们回到两个测度空间$(X,\mathcal{M},\mu),(Y,\mathcal{N},\nu)$的乘积空间，对于$E\subset X\times Y$，和$x\in X,y\in Y$我们定义$x$-section,$y$-section：
>[!Definition]
>>$E_{x}=\left\{ y\in Y:(x,y)\in E \right\},E^{y}=\left\{ x\in X:(x,y)\in E\right\}$

对于$X\times Y$上的函数$f$，定义$x$-section $f_{x}$，$y$-section $f^{y}$
>[!Definition]
>>$f_{x}(y)=f^{y}(x)=f(x,y)$

其中$f_{x}:Y\to?,f^{y}:X\to?$
>[!Example]
>>$(\mathcal{X}_{E})_{x}=\mathcal{X}_{E_{x}},(\mathcal{X}_{E})^{y}=\mathcal{X}_{E^{y}}$
[[prove 2025.02.05.20 20]]

>[!Proposition 2.34]
>a. $E\in \mathcal{M}\otimes \mathcal{N}\implies \forall x\in X,E_{x}\in \mathcal{N};\forall y\in Y,E^{y}\in \mathcal{M}$
>b. $f\ is\ \mathcal{M}\otimes \mathcal{N}-measurable\implies \forall x\in X,f_{x}\ is\ \mathcal{N}-measurable$ and$\forall y\in Y,f^{y}\ is\ \mathcal{M}-mersurable$
>>Prove

接下来介绍一个技术性引理
称$\mathcal{P}(X)$的子集$\mathfrak{C}$是单调类，若$E_{j}\in\mathfrak{C},E_{1}\subset E_{2}\subset\dots,\implies \cup E_{j}\in\mathfrak{C}$
$\sigma$-代数是单调类
单调类的任意交还是单调类[[prove 2025.02.06.16 27]]
于是对于$\varepsilon \subset \mathcal{P}(X)$,存在唯一的包含$\varepsilon$的单调类[[prove 2025.02.06.16 30]]称为$\varepsilon$生成的单调类
>[!Lemma] 2.35 The Monotone Class Lemma
>若$\mathcal{A}$是$X$上的代数，$\mathcal{A}$生成的单调类$\mathfrak{C}$和$\mathcal{A}$生成的$\sigma$-代数$\mathcal{M}$一致
>>Prove

>[!Theorem 2.36]
>设$(X,\mathcal{M},\mu),(Y,\mathcal{N},\nu)$是$\sigma$-有限测度空间，$E\in \mathcal{M}\otimes \mathcal{N}$，那么$x\to \nu(E_{x}),y\to \mu(E^{y})$是$X$和$Y$上的可测函数，并且$(\mu \times \nu)(E)=\int \nu(E_{x})d\mu(x)=\int \mu(E^{y})d\nu(y)$
>>Prove

>[!Theorem] 2.37 The Fubini-Tonelli Theorem
>设$(X,\mathcal{M},\mu),(Y,\mathcal{N},\nu)$是$\sigma$-有限的测度空间
>a. (Tonelli) $f\in L^{+}(X\times Y)\implies g(x)=\int f_{x}d\nu\ and\ h(y)=\int f^{y}d\mu$分别属于$L^{+}(X),L^{+}(Y)$
>并且$$\int fd(\mu \times \nu)=\int\left[\int f(x,y)d\nu(y) \right]d\mu(x)=\int \left[ \int f(x,y)d\mu(x) \right]d\nu(y)$$
>b. (Fubini) $f\in L^{1}(\mu \times \nu)\implies f_{x}\in L^{1}(\nu)\ for\ a.e.\ x\in X,f^{y}\in L^{1}(\mu)\ for\ a.e.\ y\in Y$，并且$$\int fd(\mu \times \nu)=\int\left[\int f(x,y)d\nu(y) \right]d\mu(x)=\int \left[ \int f(x,y)d\mu(x) \right]d\nu(y)$$
>>Prove

>[!Remark]
>* 经常做如下约定$\int \left[ \int f(x,y)d\mu(x) \right]d\nu(y)=\iint f(x,y)d\mu(x)d\nu(y)=\iint fd\mu d\nu$
>* $\sigma$-有限的假设是必要的




