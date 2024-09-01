### Problem1
设 $e_1,e_2,...,e_n$为$V$的规范正交基,并设 $v_1,...v_n\in V$,对 $\forall j=1,2,...,n$,均有$\lVert e_j-v_j\rVert<\dfrac{1}{\sqrt{n}}$.证明：$v_1,...v_n$为$V$的基.

$proof:$  设 $\sum_{i=1}^{n}a_iv_i=0,$ 假设 $\exist i\in{1,2,...,n},s.t. a_i \neq 0$.

一方面, $\lVert \sum_{i=1}^{n}a_i(e_i-v_i)\rVert ^2 = \lVert \sum_{i=1}^{n}a_ie_i\rVert ^2=\sum_{i=1}^{n} \lvert a_i\rvert^2$.

另一方面, $\lVert \sum_{i=1}^{n}a_i(e_i-v_i)\rVert^2=\lang \sum_{i=1}^{n}a_i(e_i-v_i),\sum_{i=1}^{n}a_i(e_i-v_i) \rang $

$=\sum_{i=1}^{n}\sum_{j=1}^{n} \lang a_i(e_i-v_i),a_j(e_j-v_j)\rang $

$\leqslant \sum_{i=1}^{n}\sum_{j=1}^{n}\lvert \lang a_i(e_i-v_i),a_j(e_j-v_j)\rang \rvert$

$\leqslant \sum_{i=1}^{n} \sum_{j=1}^{n} \lVert a_i(e_i-v_i)\rVert \lVert a_j(e_j-v_j)\rVert$

$=\sum_{i=1}^{n} \sum_{j=1}^{n} \lvert a_i\rvert \lvert a_j\rvert \lVert e_i-v_i\rVert \lVert e_j-v_j\rVert$

$<\dfrac{1}{n}\sum_{i=1}^{n} \sum_{j=1}^{n} \lvert a_i\rvert \lvert a_j\rvert$

$=\dfrac{1}{n} (\sum_{i=1}^{n} \lvert a_i\rvert)^2\leqslant \sum_{i=1}^{n} \lvert a_i \rvert^2$.

从而得到 $\sum_{i=1}^{n} \lvert a_i\rvert^2<\sum_{i=1}^{n} \lvert a_i\rvert^2$,矛盾.

故对 $\forall i \in {1,2,...,n},a_i=0.$

从而 $v_1,v_2,...v_n$ 线性无关,它们构成$V$的基.