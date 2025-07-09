## Calculus Problems with Data Structures in Python

## Purpose
This project was created to:
- **Understand the workings** of various data structures through solving calculus problems
- **Connect theory with practice** between data structures and mathematics
- **Develop skills in selecting** appropriate data structures for problems
- **Learn Python programming** for mathematical computation

## List of Data Structures and Applications

### Linear Data Structures

#### 1. Array/List - Numerical Integration
**Benefits:** Store function values and calculate numerical integrals
**Calculation Method:**
∫[a,b] f(x)dx ≈ Σ f(xi) × Δx
where Δx = (b-a)/n, xi = a + i×Δx

**Suitable for:** Large datasets, numerical computation

#### 2. Stack - Expression Evaluation
**Benefits:** Process mathematical expressions and calculate derivatives
**Calculation Method:**
Power Rule: d/dx(axⁿ) = n×a×xⁿ⁻¹
Use Stack to store tokens and process in order

**Suitable for:** Complex expressions, formula parsing

#### 3. Queue - Series Calculation
**Benefits:** Calculate Taylor/Maclaurin series sequentially
**Calculation Method:**
eˣ = Σ(n=0 to ∞) xⁿ/n! = 1 + x + x²/2! + x³/3! + ...
Use Queue to store terms and calculate in sequence

**Suitable for:** Series calculation, function approximation

#### 4. Linked List - Polynomial Operations
**Benefits:** Handle dynamic polynomials and calculate derivatives
**Calculation Method:**
Polynomial: a₀ + a₁x + a₂x² + ... + aₙxⁿ
Each node stores (coefficient, power)
Derivative: aᵢxⁱ → i×aᵢ×xⁱ⁻¹

**Suitable for:** Polynomials of uncertain size, adding/removing terms

### Non-Linear Data Structures

#### 5. Binary Tree - Expression Tree
**Benefits:** Represent mathematical expressions and calculate symbolic derivatives
**Calculation Method:**
Product Rule: (f×g)' = f'×g + f×g'
Each node stores operator or operand
Use recursive traversal to calculate derivatives

**Suitable for:** Complex expressions, symbolic computation

#### 6. Hash Table - Memoization
**Benefits:** Store calculated results to improve efficiency
**Calculation Method:**
factorial(n) = n × factorial(n-1)
Store results in hash table
Time: O(1) for already calculated values

**Suitable for:** Repeated calculations, series, optimization

#### 7. Heap - Optimization
**Benefits:** Find maximum/minimum points in optimization problems
**Calculation Method:**
Critical Points: f'(x) = 0
Max Heap: store maximum values (use negative values)
Min Heap: store minimum values

**Suitable for:** Finding extrema, optimization problems

#### 8. Graph - Gradient Descent
**Benefits:** Show paths for finding optimal values
**Calculation Method:**
Gradient Descent: xₙ₊₁ = xₙ - α×f'(xₙ)
α = learning rate
Each node is a point in solution space

**Suitable for:** Machine learning, optimization networks

#### 9. Trie - Pattern Matching
**Benefits:** Match expression patterns with derivative rules
**Calculation Method:**
Pattern: "x^n" → Rule: "Power Rule"
Store patterns in trie structure
Search: O(m) where m = pattern length

**Suitable for:** Computational assistant systems, pattern recognition

## Usage Instructions

### Installation
```bash
pip install numpy matplotlib
```

### Running the Code
```python
# Run section by section or run all
python calculus_data_structures.py
```

### Usage Examples
```python
# Calculate integral with Array
integral, x_vals, y_vals = riemann_sum(lambda x: x**2, 0, 2, 100)

# Calculate derivative with Stack
calc = DerivativeCalculator()
derivative = calc.derivative_power_rule("3x^2")

# Calculate Taylor Series with Queue
approx_e = taylor_series_queue(1.0, 10)
```

## Performance Comparison

| Data Structure | Time Complexity | Space Complexity | Best Use Case |
|---|---|---|---|
| Array | O(n) | O(n) | Large datasets |
| Stack | O(n) | O(n) | Complex expressions |
| Queue | O(n) | O(n) | Sequential processing |
| Linked List | O(n) | O(n) | Dynamic polynomials |
| Binary Tree | O(log n) | O(n) | Symbolic computation |
| Hash Table | O(1) avg | O(n) | Memoization |
| Heap | O(log n) | O(n) | Optimization |
| Graph | O(V+E) | O(V+E) | Network optimization |
| Trie | O(m) | O(ALPHABET×N) | Pattern matching |

## What We Learned

### Data Structures:
- **Selecting** appropriate structures for problems
- **Trade-offs** between time and space complexity
- **Practical applications** in real situations

### Calculus:
- **Numerical methods** for integral calculation
- **Symbolic differentiation** with tree structures
- **Optimization algorithms** and finding extrema
- **Series approximation** and convergence

**Note:** This project is suitable for those with high school level mathematics background and basic Python programming knowledge.
