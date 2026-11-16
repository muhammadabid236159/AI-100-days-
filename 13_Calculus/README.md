# 📊 Calculus for Machine Learning

Calculus Machine Learning ki rooh (soul) hai — Gradient Descent se le kar Backpropagation tak, sab Calculus pe based hain.

---

## 📚 Key Topics & Notebook Content:

### 1️⃣ Limits ($\lim_{x \to a} f(x)$)
- Derivative ki foundational definition limits se aati hai
- Numerical approach: $h \to 0$ mein secant line tangent ban jati hai

### 2️⃣ Derivatives — $f'(x)$ (Rate of Change)
- Power, Product, Chain Rule
- **ML Use:** Loss function ka slope = gradient

### 3️⃣ Partial Derivatives ($\frac{\partial f}{\partial x}$)
- Multi-variable functions mein har variable ke respect mein derivative
- **ML Use:** Backpropagation across all weights

### 4️⃣ Gradient ($\nabla f$)
- Vector of all partial derivatives
- Points in direction of steepest ascent
- **ML Use:** Tells optimizer which direction to move

### 5️⃣ Gradient Descent
- Iterative algorithm to minimize loss: $w \leftarrow w - \alpha \nabla L$
- Learning rate $\alpha$ effect visualization

### 6️⃣ Integration ($\int f(x) dx$)
- Anti-derivative and area under curve
- Riemann Sum numerical approximation
- **ML Use:** Probability, Expected Value, KL Divergence

### 7️⃣ Chain Rule & Backpropagation
- Composite function derivatives
- Manual neural network backprop simulation
- Sigmoid derivative visualization

---

## 💻 Notebook:
Run [`day30_calculus.ipynb`](day30_calculus.ipynb) for complete code, formulas, and visualizations.
