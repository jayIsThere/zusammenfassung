+++
title = 'Vektor- und Matrix-Formeln'
date = 2025-03-01T18:33:36+02:00
categories = ['SLA']
tags = ['Vektor', 'Matrix', 'Determinant']
draft = false
math = true
+++

### Vektor-Formeln

1. **Skalarprodukt (Dot Product)**  
   Das Skalarprodukt von zwei Vektoren \( \mathbf{u}, \mathbf{v} \in \mathbb{R}^n \) ist definiert als:
   $$
   \mathbf{u} \cdot \mathbf{v} = \sum_{i=1}^{n} u_i v_i
   $$

   <img src="/../images/skalarprodukt.jpg" width="450px" height="430px">

2. **Vektorlänge (Norm)**  
   Die Länge (Norm) eines Vektors \( \mathbf{a} \in \mathbb{R}^n \) ist gegeben durch:
   $$
   |\mathbf{a}| = \sqrt{a_1^2 + a_2^2 + \dots + a_n^2}
   $$

   <img src="{{ site.baseurl }}/vektorlaenge.jpg" width="450px" height="430px">

3. **Winkel zwischen Vektoren (Angle between Vectors)**  
   Der Winkel \( \theta \) zwischen den Vektoren \( \mathbf{a}, \mathbf{b} \in \mathbb{R}^n \) wird durch die folgende Formel berechnet:
   $$
   \cos(\theta) = \frac{\mathbf{a} \cdot \mathbf{b}}{|\mathbf{a}| |\mathbf{b}|}
   $$

   <img src="{{ site.baseurl }}/winkel.jpg" width="450px" height="430px">

4. **Orthogonalität (Orthogonality)**  
   Zwei Vektoren \( \mathbf{a} \) und \( \mathbf{b} \) sind orthogonal (rechtwinklig), wenn:
   $$
   \mathbf{a} \cdot \mathbf{b} = 0
   $$

   <img src="{{ site.baseurl }}/orthogonal.jpg" width="450px" height="430px">

5. **Kreuzprodukt (Cross Product) - In 3D**  
   Das Kreuzprodukt zweier Vektoren $$ \mathbf{a} = (a_1, a_2, a_3) $$ und $$ \mathbf{b} = (b_1, b_2, b_3)$$  ist:
   $$
   \mathbf{a} \times \mathbf{b} = 
   \begin{vmatrix}
   \mathbf{i} & \mathbf{j} & \mathbf{k} \\
   a_1 & a_2 & a_3 \\
   b_1 & b_2 & b_3
   \end{vmatrix}
   = \left( a_2 b_3 - a_3 b_2, \, a_3 b_1 - a_1 b_3, \, a_1 b_2 - a_2 b_1 \right)
   $$

   <img src="{{ site.baseurl }}/kreuzprodukt.jpg" width="450px" height="430px">

---

### Matrix-Formeln

1. **Matrixmultiplikation (Matrix Multiplication)**  
   Die Multiplikation zweier Matrizen \( A \in \mathbb{R}^{m \times n} \) und \( B \in \mathbb{R}^{n \times p} \) ergibt:
   $$
   C = AB, \quad C_{ij} = \sum_{k=1}^{n} A_{ik} B_{kj}
   $$

   <img src="{{ site.baseurl }}/matrix_multiplikation.jpg" width="450px" height="430px">

2. **Transponierte Matrix (Transpose of a Matrix)**  
   Die Transponierte einer Matrix \( A = [a_{ij}] \) ist:
   $$
   A^T = [a_{ji}]
   $$

3. **Determinante einer Matrix (Determinant of a Matrix)**  
   Die Determinante einer 2x2-Matrix $$ A = \begin{pmatrix} a & b \\ c & d \end{pmatrix} $$ ist:
   $$
   \det(A) = ad - bc
   $$

4. **Inverse Matrix (Inverse Matrix)**  
   Wenn die Matrix \( A \) invertierbar ist, dann ist die Inverse von \( A \):
   $$
   A^{-1} = \frac{1}{\det(A)} \text{adj}(A)
   $$
   wobei $$ \text{adj}(A) $$ die adjungierte Matrix von \( A \) ist.
   
5. **Eigenwerte und Eigenvektoren (Eigenvalues and Eigenvectors)**  
   Die Eigenwerte \( \lambda \) und Eigenvektoren \( \mathbf{v} \) einer Matrix \( A \) erfüllen die Gleichung:
   $$
   A \mathbf{v} = \lambda \mathbf{v}
   $$

6. **Lösung eines linearen Systems (Solution of a Linear System)**  
   Die Lösung des linearen Systems \( A \mathbf{x} = \mathbf{b} \) ist:
   $$
   \mathbf{x} = A^{-1} \mathbf{b}, \quad \text{wenn } A \text{ invertierbar ist.}
   $$

---
