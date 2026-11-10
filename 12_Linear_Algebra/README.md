# 📐 Linear Algebra & Coordinate Geometry for Machine Learning

Linear Algebra and Coordinate Geometry form the foundational mathematical backbone for Machine Learning (Regression, Support Vector Machines, PCA, Computer Vision, and Deep Neural Networks).

---

## 📚 Key Topics & Notebook Content:

### 1️⃣ Distance Between Two Points ($L_2$ Euclidean Distance)
- **Concept:** Shortest straight line connecting two coordinate points $P_1(x_1, y_1)$ and $P_2(x_2, y_2)$.
- **Formula:**
  $$d = \sqrt{(x_2 - x_1)^2 + (y_2 - y_1)^2}$$
- **ML Use Case:** KNN classification, K-Means clustering, distance loss functions.

---

### 2️⃣ Straight Lines (Linear Equations)
- **Concept:** A constant rate of change between $x$ and $y$.
- **Slope-Intercept Form:**
  $$y = mx + c$$
  Where $m = \frac{\Delta y}{\Delta x} = \text{slope}$ and $c = \text{Y-intercept}$.
- **General Form:**
  $$Ax + By + C = 0 \implies m = -\frac{A}{B}, \quad c = -\frac{C}{B}$$
- **ML Use Case:** Linear Regression line $\hat{y} = w_1 x + b$, decision boundaries.

---

### 3️⃣ Parallel Lines & Distance Between Parallel Lines
- **Concept:** Lines with identical slopes ($m_1 = m_2$) that never meet.
- **Shortest Perpendicular Distance Formula:**
  $$d = \frac{|c_1 - c_2|}{\sqrt{1 + m^2}} \quad \text{or} \quad d = \frac{|C_1 - C_2|}{\sqrt{A^2 + B^2}}$$
- **ML Use Case:** Margin calculation and hyperplane separation in Support Vector Machines (SVM).

---

### 4️⃣ Perpendicular Lines (Orthogonality)
- **Concept:** Lines meeting at a $90^\circ$ right angle. Slopes are negative reciprocals.
- **Condition:**
  $$m_1 \cdot m_2 = -1 \implies m_2 = -\frac{1}{m_1}$$
- **ML Use Case:** Orthogonal projections, dot product $= 0$, Principal Component Analysis (PCA) eigenvectors.

---

### 5️⃣ Vector Addition & Geometric Visualizations
- **Concept:** Adding corresponding components of vectors ($\mathbf{u} + \mathbf{v}$).
- **Geometric Methods:**
  - **Head-to-Tail Rule (Triangle Law):** Tail of $\mathbf{v}$ placed at head of $\mathbf{u}$.
  - **Parallelogram Law:** Both vectors start from origin, diagonal represents resultant.
- **ML Use Case:** Word embeddings (Word2Vec: $\vec{v}_{\text{King}} - \vec{v}_{\text{Man}} + \vec{v}_{\text{Woman}} \approx \vec{v}_{\text{Queen}}$), neural network layer activations ($W\mathbf{x} + \mathbf{b}$).

---

### 6️⃣ Vector Scalar Multiplication & 3D Scaling Visuals
- **Concept:** Multiplying each element of a vector by a scalar constant $c \cdot \mathbf{v}$.
- **3D Example:**
  $$\mathbf{v} = \begin{bmatrix} 2 \\ 1 \\ 3 \end{bmatrix}, \quad c = 3 \implies \text{Resultant} = \begin{bmatrix} 6 \\ 3 \\ 9 \end{bmatrix}$$
- **Geometric Effect:** Stretches the vector by factor of $3$ while maintaining identical direction in 3D space.
- **ML Use Case:** Learning rate scaling in Gradient Descent, feature scaling / normalization.

---

### 7️⃣ Cross Product (Vector Product) & 3D Visuals
- **Concept:** Defined strictly in 3D space. The result of $\mathbf{u} \times \mathbf{v}$ is a **NEW 3D vector** that is strictly **perpendicular ($90^\circ$)** to both input vectors.
- **Formulas:**
  - **Magnitude / Parallelogram Area:** $\|\mathbf{u} \times \mathbf{v}\| = \|\mathbf{u}\| \|\mathbf{v}\| \sin(\theta)$
  - **Determinant Form:**
    $$\mathbf{u} \times \mathbf{v} = \det \begin{bmatrix} \mathbf{i} & \mathbf{j} & \mathbf{k} \\ u_1 & u_2 & u_3 \\ v_1 & v_2 & v_3 \end{bmatrix} = \begin{bmatrix} u_2 v_3 - u_3 v_2 \\ u_3 v_1 - u_1 v_3 \\ u_1 v_2 - u_2 v_1 \end{bmatrix}$$
  - **Anti-commutative Property:** $\mathbf{v} \times \mathbf{u} = -(\mathbf{u} \times \mathbf{v})$
- **ML Use Case:** Surface normal estimation in 3D Computer Vision, NeRFs, Point Cloud processing, and Robotics kinematics.

---

### 8️⃣ Determinants of Matrices ($\det(A)$ or $|A|$)
- **Concept:** A scalar property calculated only for square matrices.
- **Geometric Meaning:** Represents the **Area Scaling Factor** (2D) or **Volume Scaling Factor** (3D) under matrix transformation.
  - Unit square of area $1$ transforms to a parallelogram of area $|\det(A)|$.
  - If $\det(A) = 0$, space is squashed to a 1D line $\implies$ matrix is **Singular** (has no inverse!).
- **Formulas:**
  - $2 \times 2$: $\det \begin{bmatrix} a & b \\ c & d \end{bmatrix} = ad - bc$
  - $3 \times 3$: $\det \begin{bmatrix} a & b & c \\ d & e & f \\ g & h & i \end{bmatrix} = a(ei - fh) - b(di - fg) + c(dh - eg)$
- **ML Use Case:** Covariance matrix determinant in Multivariate Gaussian distributions, Normalizing Flows Jacobian determinant, PCA eigenvalues.

---

### 9️⃣ Matrix Inversion & Foundations (Dot Product & Linear Systems)
- **Concept:** Core primitives of linear transformations:
  - Vector dot product $\mathbf{u} \cdot \mathbf{v} = \sum u_i v_i$ ($\mathbf{u} \cdot \mathbf{v} = 0 \iff$ orthogonal)
  - Matrix inverse $A^{-1} = \frac{1}{\det(A)} \operatorname{adj}(A)$ (Requires $\det(A) \neq 0$)
  - Verification: $A \cdot A^{-1} = I$ (Identity Matrix)
- **ML Use Case:** Normal Equation in Linear Regression $\mathbf{w} = (X^T X)^{-1} X^T \mathbf{y}$, weight inversion, linear systems solver.

---

### 🔟 Vector Projection & Orthogonality
- **Concept:** Projecting vector $\mathbf{v}$ onto base vector $\mathbf{u}$ (shadow calculation):
  $$\operatorname{proj}_{\mathbf{u}}(\mathbf{v}) = \left(\frac{\mathbf{u} \cdot \mathbf{v}}{\|\mathbf{u}\|^2}\right) \mathbf{u}$$
  Perpendicular error component $\mathbf{v}_{\perp} = \mathbf{v} - \operatorname{proj}_{\mathbf{u}}(\mathbf{v})$ has $\mathbf{v}_{\perp} \cdot \mathbf{u} = 0$.
- **ML Use Case:** Dimensionality reduction, Cosine similarity, SVM hyperplane projection.

---

### 1️⃣1️⃣ Eigenvalues & Eigenvectors ($A\mathbf{v} = \lambda \mathbf{v}$)
- **Concept:** Vectors whose direction remains unchanged under transformation $A$; they only get scaled by factor $\lambda$:
  $$\det(A - \lambda I) = 0$$
- **ML Use Case:** Principal Component Analysis (PCA directions of maximum variance), Google PageRank, Spectral Clustering, Singular Value Decomposition (SVD).

---

## 💻 Notebook Implementation:
- Open and run [`day29_linear_algebra.ipynb`](day29_linear_algebra.ipynb) for all detailed explanations, formulas, runnable Python code, and rich 2D & 3D Matplotlib visualizations.
