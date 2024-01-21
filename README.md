# Maths

#### Problem 1 (Mathematical induction)
Let $n \geq 1$. Prove that $$\sum_{j=1}^n (-1)^{j-1}j^2=(-1)^{n-1}\frac{n(n+1)}{2}$$

**Base case**:

For $n=1$.

$$\sum_{j=1}^1(-1)^{1-1}1^2=1=(-1)^{1-1}\frac{1(1+1)}{2}= 1\frac{2}{2}=1$$

**Inductive steps** (Inductive Hypothesis) Assume that the result is true for $n=k$ where $k\geq 1$ :

$$\sum_{j=1}^k(-1)^{j-1}1^2=(-1)^{k-1}\frac{k(k+1)}{2}$$
Now let's assume that the result is also true for $n=k+1$ where $k\geq 1$. 
$$\sum_{j=1}^{k+1}(-1)^{j-1}j^2=(-1)^{k}\frac{(k+1)(k+2)}{2}$$
Assume that $k \geq 1$ Then:

$$\sum_{j=1}^{k+1}(-1)^{j-1}j^2$$
$=$
$$\sum_{j=1}^{k}(-1)^{j-1}j^2+(-1)^k(k+1)^2$$
$=$
$$(-1)^{k-1}\frac{k(k+1)}{2}+(-1)^k(k+1)^2$$
$=$
$$(-1)^k\left((k+1)^2+(-1)^{-1}\frac{k(k+1)}{2}\right)$$
$=$
$$(-1)^k\left(\frac{2(k+1)^2+(-k)(k+1)}{2}\right)$$
$=$
$$(-1)^k\frac{(k+1)(2(k+1)-k)}{2}$$
$=$
$$(-1)^k\frac{(k+1)(2k+2-k)}{2}$$
$=$
$$(-1)^k\frac{(k+1)(k+2)}{2}$$
By Principle of Mathematical induction this equation $$\sum_{j=1}^{k+1}(-1)^{j-1}j^2=(-1)^{k}\frac{(k+1)(k+2)}{2}$$ holds for all $n\in \mathbb{N}$. 

#### Problem 2 (Formula demonstration)

Prove that: $$\Vert x \Vert \times \Vert y \Vert \times \cos\theta = \sum_{n=0}^{n-1} \chi_i\Psi_i$$
Demonstration:
$$\Vert x \Vert \times \Vert y \Vert \times \cos\theta$$
$$\Leftrightarrow\sqrt{\sum_{i=0}^{n-1}\chi_i^2}\times\sqrt{\sum_{i=0}^{n-1}\Psi_i^2}\times\cos\theta $$

$$\Leftrightarrow\sqrt{\sum_{i=0}^{n-1}\chi_i^2}\times\sqrt{\sum_{i=0}^{n-1}\Psi_i^2}\times\frac{\sum_{i=0}^{n-1} \chi_i\Psi_i}{\sqrt{\sum_{i=0}^{n-1}\chi_i^2}\times\sqrt{\sum_{i=0}^{n-1}\Psi_i^2}}$$
$$\Leftrightarrow\sum_{n=0}^{n-1} \chi_i\Psi_i$$

So $\Vert x \Vert \times \Vert y \Vert \times \cos\theta = \sum_{n=0}^{n-1} \chi_i\Psi_i$

This demonstration was made to show why when we have coordinates you can simply compute the dot product like this $\sum_{n=0}^{n-1} \chi_i\Psi_i$ and that you are not obligated to use this formula $\Vert x \Vert \times \Vert y \Vert \times \cos\theta$.
