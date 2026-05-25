# Linear Algebra

## Basic idea

Linear maps between vector spaces are fully described by matrices once a basis is fixed. Most computations reduce to multiplication, inversion, and eigen-decomposition.

## Key formulas

- Matrix multiplication: $(AB)_{ij}=\sum_k A_{ik}B_{kj}$
- Dot product: $\mathbf{a}\cdot\mathbf{b}=\sum_i a_i b_i = \|\mathbf{a}\|\|\mathbf{b}\|\cos\theta$
- Norm ($L^2$): $\|\mathbf{x}\|_2=\sqrt{\sum_i x_i^2}$
- Determinant (2x2): $\det\begin{pmatrix}a&b\\c&d\end{pmatrix}=ad-bc$
- Inverse exists $\iff \det A \ne 0$; $A^{-1}=\dfrac{1}{\det A}\operatorname{adj}(A)$
- Eigenvalue equation: $Av=\lambda v$, characteristic polynomial $\det(A-\lambda I)=0$
- Trace: $\operatorname{tr}(A)=\sum_i A_{ii}=\sum_i \lambda_i$
- Rank-nullity: $\operatorname{rank}(A)+\operatorname{nullity}(A)=n$
- Singular value decomposition: $A=U\Sigma V^\top$
- Cauchy-Schwarz: $|\langle u,v\rangle|\le\|u\|\|v\|$

