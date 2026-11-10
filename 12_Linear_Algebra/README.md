# 📐 Linear Algebra & Coordinate Geometry for Machine Learning

Linear Algebra and Coordinate Geometry form the foundational backbone for Machine Learning (Regression, Support Vector Machines, PCA, and Neural Networks).

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
- **ML Use Case:** Linear Regression line $\hat{y} = w_1 x + b$.

---

### 3️⃣ Parallel Lines & Distance Between Parallel Lines
- **Concept:** Lines with identical slopes ($m_1 = m_2$) that never meet.
- **Shortest Perpendicular Distance Formula:**
  $$d = \frac{|c_1 - c_2|}{\sqrt{1 + m^2}} \quad \text{or} \quad d = \frac{|C_1 - C_2|}{\sqrt{A^2 + B^2}}$$
- **ML Use Case:** Margin calculation in Support Vector Machines (SVM).

---

### 4️⃣ Perpendicular Lines (Orthogonality)
- **Concept:** Lines meeting at a $90^\circ$ right angle. Slopes are negative reciprocals.
- **Condition:**
  $$m_1 \cdot m_2 = -1 \implies m_2 = -\frac{1}{m_1}$$
- **ML Use Case:** Orthogonal projection, dot product $= 0$, Principal Component Analysis (PCA).

---

## 💻 Notebook Implementation:
- Run [`day29_linear_algebra.ipynb`](day29_linear_algebra.ipynb) for runnable Python code, formulas, and 2D Matplotlib visualizations.
