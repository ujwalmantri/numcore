# 🧮 numcore

A comprehensive mathematics library built from scratch by a first-year student. Growing daily with new functions across statistics, number theory, linear algebra, and more.

[![PyPI version](https://badge.fury.io/py/numcore.svg)](https://pypi.org/project/numcore/)
[![Python](https://img.shields.io/badge/python-3.7+-blue.svg)](https://www.python.org/downloads/)

## 🚀 Installation

```bash
pip install numcore
```

## 📖 Usage

### **Statistical Analysis**
```python
from numcore import (mean, median, std, analyze_list, covariance, 
                     z_score, coefficient_of_variation)

data = [23, 45, 67, 45, 89, 34, 78, 98, 54, 55]
print(mean(data))      # 58.8
print(std(data))       # 23.82

# Advanced stats
print(z_score(75, data))                    # Standard score
print(coefficient_of_variation(data))       # Relative variability
print(covariance([1,2,3], [2,4,6]))        # Covariance
```

### **Means (Arithmetic, Geometric, Harmonic)**
```python
from numcore import mean, geometric_mean, harmonic_mean

data = [2, 4, 8]
print(mean(data))             # 4.67 (arithmetic)
print(geometric_mean(data))   # 4.0 (geometric)
print(harmonic_mean(data))    # 3.43 (harmonic)
```

### **Number Theory**
```python
from numcore import (is_prime, gcd, euler_totient, mobius,
                     legendre_symbol, is_coprime, catalan_number)

print(is_prime(17))          # True
print(euler_totient(9))      # 6
print(mobius(30))            # -1
print(is_coprime(8, 15))     # True
print(catalan_number(5))     # 42
```

### **Sequences**
```python
from numcore import (fibonacci, arithmetic_seq, geometric_seq,
                     lucas, collatz, harmonic_series)

print(fibonacci(10))            # [0, 1, 1, 2, 3, 5, 8, 13, 21, 34]
print(arithmetic_seq(2, 3, 5))  # [2, 5, 8, 11, 14]
print(geometric_seq(2, 3, 4))   # [2, 6, 18, 54]
print(harmonic_series(5))       # 2.283... (1 + 1/2 + 1/3 + 1/4 + 1/5)
```

### **Combinatorics & Probability**
```python
from numcore import npr, ncr, binomial_coeff

print(npr(5, 3))           # 60 (permutations)
print(ncr(5, 3))           # 10 (combinations)
print(binomial_coeff(5, 2)) # 10 (same as ncr)
```

### **Financial Mathematics**
```python
from numcore import rate_of_return

print(rate_of_return(110, 100))  # 10.0% gain
print(rate_of_return(90, 100))   # -10.0% loss
```

## ✨ Features

### **Input Functions (2)**
- `n_input(n)` - Get n integers with validation
- `input_matrix()` - Interactive matrix input

### **Basic Statistics (6)**
- `mean(lst)` - Arithmetic mean
- `median(lst)` - Middle value
- `mode(lst)` - Most common value(s)
- `variance(lst, sample)` - Variance
- `std(lst, sample)` - Standard deviation
- `analyze_list(lst)` - Comprehensive analysis

### **Advanced Statistics (7)**
- `geometric_mean(lst)` - Geometric mean
- `harmonic_mean(lst)` - Harmonic mean
- `covariance(lst1, lst2)` - Covariance
- `z_score(x, lst)` - Standard score
- `percentile(lst, p)` - pth percentile value
- `coefficient_of_variation(lst)` - Relative variability (CV)
- `mean_absolute_deviation(lst)` - MAD

### **Number Theory (22)**
- `factorial(n)`, `nth_root(num, n)`
- `divisors(num)`, `proper_divisors(num)`, `common_divisors(a,b)`
- `gcd(a, b)`, `lcm(a, b)`
- `is_prime(num)`, `primes(num)`
- `prime_divisors(num)`, `prime_factorization(num)`, `prime_factors(num)`
- `is_perfect(num)`, `is_armstrong(num)`, `is_amicable(a,b)`
- `euler_totient(num)` - Euler's φ function
- `mobius(num)` - Möbius μ function
- `quadratic_residue(num)`, `quadratic_non_residue(num)`
- `legendre_symbol(a, p)` - Legendre symbol
- `is_coprime(a, b)` - Check if coprime
- `catalan_number(n)` - nth Catalan number

### **Sequences (15)**
- **Fibonacci:** `fibonacci(n)`, `nth_fibonacci(n)`
- **Lucas:** `lucas(n)`, `nth_lucas(n)`
- **Arithmetic:** `arithmetic_seq(a,d,n)`, `nth_arithmetic(a,d,n)`, `arithmetic_sum(a,d,n)`
- **Geometric:** `geometric_seq(a,r,n)`, `nth_geometric(a,r,n)`, `geometric_sum(a,r,n)`
- **Harmonic:** `harmonic_seq(a,d,n)`, `nth_harmonic(a,d,n)`, `harmonic_sum(a,d,n)`
- **Special:** `collatz(n)`, `farey(num)`, `harmonic_series(n)`

### **Combinatorics (3)**
- `npr(n, r)` - Permutations
- `ncr(n, r)` - Combinations
- `binomial_coeff(n, k)` - Binomial coefficient

### **Digit Operations (3)**
- `digits(num)` - Extract digits as list
- `reverse_number(num)` - Reverse digits
- `sum_of_digits(num)` - Sum all digits

### **List Utilities (4)**
- `counter(lst)` - Count occurrences
- `product(lst)` - Multiply all elements
- `power_list(lst, power)` - Apply power to each
- `reciprocal_list(lst)` - Calculate reciprocals

### **Basic Matrix Operations (8)**
- `create_matrix(rows, cols, fill)` - Create matrix
- `matrix_shape(matrix)` - Get dimensions
- `matrix_add(mat1, mat2)` - Addition
- `matrix_sub(mat1, mat2)` - Subtraction
- `scalar_multiply(matrix, scalar)` - Scalar multiplication
- `matrix_multiply(mat1, mat2)` - Matrix multiplication
- `print_matrix(matrix)` - Pretty print

### **Advanced Matrix Operations (9)**
- `matrix_identity(n)` - Identity matrix
- `matrix_transpose(matrix)` - Transpose
- `matrix_trace(matrix)` - Trace
- `determinant(matrix)` - Determinant (recursive)
- `matrix_minor(matrix)` - Matrix of minors
- `matrix_cofactor(matrix)` - Cofactor matrix
- `matrix_power(matrix, n)` - Matrix exponentiation
- `is_square(matrix)` - Check if square
- `is_orthogonal(matrix)` - Check orthogonality

### **Utility Functions (2)**
- `signum(x)` - Sign function
- `rate_of_return(current, original)` - Financial return %

## 🎯 Roadmap

- [x] Statistical analysis (basic & advanced)
- [x] Number theory suite
- [x] Sequence generation
- [x] Matrix operations (basic & advanced)
- [x] Combinatorics
- [ ] Trigonometry (sin, cos, tan with degrees)
- [ ] Linear algebra (eigenvalues, decomposition)
- [ ] Calculus (derivatives, integrals)
- [ ] Probability distributions
- [ ] Graph theory
- [ ] Optimization algorithms
- [ ] And more... continuously growing!

## 📊 Current Library

**Total Functions:** 84

Growing daily with new mathematical capabilities!

## 💡 Example Use Cases

### **Portfolio Analysis**
```python
from numcore import rate_of_return, mean, std

returns = [5.2, -2.1, 8.3, 3.4, -1.5]
avg_return = mean(returns)
volatility = std(returns)
print(f"Average: {avg_return}%, Volatility: {volatility}%")
```

### **Data Science: Z-Scores**
```python
from numcore import z_score

exam_scores = [72, 85, 90, 65, 88, 92, 78]
your_score = 88

z = z_score(your_score, exam_scores)
print(f"Your z-score: {z:.2f}")  # How many std devs above/below mean
```

### **Catalan Numbers (Binary Trees)**
```python
from numcore import catalan_number

# How many different binary trees with n nodes?
for n in range(6):
    print(f"{n} nodes: {catalan_number(n)} trees")
# 0: 1, 1: 1, 2: 2, 3: 5, 4: 14, 5: 42
```

### **Covariance (Relationship Between Variables)**
```python
from numcore import covariance

hours_studied = [2, 4, 6, 8, 10]
exam_scores = [55, 65, 75, 85, 95]

cov = covariance(hours_studied, exam_scores)
print(f"Covariance: {cov}")  # Positive = both increase together
```

## 🛠️ Development

### **Requirements**
- Python 3.7+
- No external dependencies!

### **Organization**
Functions are organized by category for easy navigation and use.

## 📝 License

MIT License - see [LICENSE](LICENSE) file for details

## 👨‍💻 Author

**Ujwal Mantri**
- PyPI: [numcore](https://pypi.org/project/numcore/)
- GitHub: [ujwalmantri](https://github.com/ujwalmantri/numcore)
- Email: ujwalmantrifr@gmail.com

## 🌟 Support

If you find this helpful:
- ⭐ Star on GitHub
- 📦 `pip install numcore`
- 📢 Share with others

## 🎓 Learning Journey

### **Milestones**
- ✅ Published to PyPI
- ✅ 84+ functions implemented
- ✅ Advanced statistics suite
- ✅ Complete sequence generation
- ✅ Graduate-level number theory
- 🎯 Next: Organizing into modules
- 🔄 Continuously adding new functions

### **What Makes This Special**
- Built from scratch by first-year student
- Pure Python (zero dependencies)
- Comprehensive documentation
- Real mathematical algorithms
- Open source learning resource
- **Growing daily!**

## 📚 Function Categories

| Category | Count | Status |
|----------|-------|--------|
| Statistics | 13 | ✅ Comprehensive |
| Number Theory | 22 | 🔄 Growing |
| Sequences | 15 | ✅ Complete |
| Combinatorics | 3 | 🔄 Growing |
| Matrix Operations | 17 | ✅ Complete |
| List Utilities | 4 | ✅ Complete |
| Digit Operations | 3 | ✅ Complete |
| Financial Math | 1 | 🔄 Starting |
| Utilities | 2 | 🔄 Starting |
| Input/Output | 2 | ✅ Complete |
| **Total** | **84+** | **🔄 Active Development** |

---

Crafted with Python. Powered by curiosity. Open-sourced for learning. ⚡