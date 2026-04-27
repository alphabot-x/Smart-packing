# Smart Packing System 📦

A high-efficiency packing optimizer that utilizes **Dynamic Programming** to determine the most space-efficient way to pack items into a container. This system ensures maximum utility of available volume while respecting weight or priority constraints.

---

## 🚀 Overview

The **Smart Packing System** solves the combinatorial optimization problem of "what fits best?" instead of "what fits next?" By using a **DP Table** (Bottom-Up approach), the algorithm evaluates every possible sub-capacity to guarantee a mathematically optimal solution.

### Key Features
* **Optimal Space Utilization:** Uses DP to find the absolute best combination of items.
* **Constraint Management:** Supports limits on both weight and volume.
* **Performance:** Operates at $O(n \cdot W)$ time complexity, where $n$ is the number of items and $W$ is the maximum capacity.

---

## 🧠 How it Works: The DP Approach

The core of this system is the **2D Dynamic Programming Table**. The algorithm populates a matrix where:
* **Rows** represent the items available to pack.
* **Columns** represent the incremental capacity of the container.

### The Recurrence Relation
For each cell in the table, the system decides whether to include an item by evaluating:

$$DP[i][w] = \max(DP[i-1][w], \text{value}_i + DP[i-1][w - \text{weight}_i])$$

This ensures that the packing logic provides a mathematical guarantee of the best possible value for the given constraints.

---

## 🛠️ Installation & Usage

1. **Clone the repository:**
   ```bash
   git clone [https://github.com/alphabot-x/Smart-packing.git](https://github.com/alphabot-x/Smart-packing.git)
