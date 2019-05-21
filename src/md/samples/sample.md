# sample

## sample

### sample

sample

##### Example 1.1.6

> $\sigma \langle \mathcal{O}_2 \rangle = \langle \mathcal{O}_4 \rangle = \mathcal{B}(\mathbb{R})^k$

$\mathcal{G}$​を$\mathcal{O}_4$を含む$\sigma$-algebraだとする.
このとき$\mathbb{R}^k$の任意の開集合$A \subset \mathbb{R}^k$をとると,Problem1.9より$\{B_n\}_{n \ge 1} \subset \mathcal{O}_3$が存在して,$A = \bigcup_{n \ge 1} B_n$とできる.
ここで,
$B_n = (a_1^n, b_1^n) \times \cdots \times (a_k^n, b_k^n)$
とおくと,
$$
\begin{align*}
	B_n &= (a_1^n, b_1^n) \times \cdots \times (a_k^n, b_k^n)\\
		&= \bigcup_{i \ge 1} (-\infty, b_1^n) \times \cdots \times (-\infty, b_k^n) \setminus
			(-\infty, a_1^n + \frac{1}{i}) \times \cdots \times (-\infty, a_k^n + \frac{1}{i})\\
		&= \bigcup_{i \ge 1} C_n \setminus C_n^i
\end{align*}
$$
ゆえに,$A = \bigcup_{n \ge 1} \bigcup_{i \ge 1} C_n \cap (C_n^i)^c$.
$C_n, C_n^i \in \mathcal{O}_4$であり,$\mathcal{G}$は$\mathcal{O}_4$を含む$\sigma$-algebraなので$A \in \mathcal{G}$.
ゆえに,$\mathcal{G}$は$\mathbb{R}^k$の任意の開集合を含む$\sigma$-algebraであるので以下が成立
$$
\mathcal{B}(\mathbb{R}^k) \supset 
	\sigma \langle \mathcal{O}_2 \rangle \supset 
	\sigma \langle \mathcal{O}_4 \rangle =
	\bigcap_{\mathcal{G}: \mathcal{O}_4 \subset \mathcal{G}, \sigma - field}
		\mathcal{G} \supset
	\mathcal{B}(\mathbb{R}^k)
$$

##### Theorem 1.1.2 (The $\pi\text{-}\lambda$ theorem)

> $\lambda_1(\mathcal{C})$ is $\lambda$-system

Proof.
(i)$\Omega \in \lambda_1(C)$は明らか.
(ii) $A, A' \in \lambda_1(\mathcal{C}), A \subset A' \Rightarrow A' \setminus A \in \lambda_1(\mathcal{C})$を示す.
$A, A' \in \lambda_1(C)$より$A, A' \in \lambda \langle \mathcal{C} \rangle$であり, $ A \subset A' $であることを踏まえると,$A' \setminus A \in \lambda\langle \mathcal{C} \rangle$.
また,任意の$B \in \mathcal{C}$をとったとき,$(A' \setminus A) \cap B = (A' \cap B) \setminus (A \cap B) \in \lambda\langle \mathcal{C} \rangle$
(iii)$A_n \in \lambda_1(\mathcal{C}), A_n \subset A_{n+1} \Rightarrow \bigcup_n A_n \in \lambda_1(\mathcal{C})$
任意の$B \in \mathcal{C}$をとったとき,$(\bigcup_n A_n) \cap B = \bigcup_n (A_n \cap B) \in \lambda \langle \mathcal{C} \rangle$($A_n \cap B \subset A_{n+1} \cap B$)

> by the previous step $\mathcal{C} \subset \lambda_1(\mathcal{C})$

