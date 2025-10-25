# 🧮 numcore

A comprehensive mathematics library built from scratch by a first-year student. Currently in active development with a goal of **250+ functions**.

[![PyPI version](https://badge.fury.io/py/numcore.svg)](https://pypi.org/project/numcore/)
[![Python](https://img.shields.io/badge/python-3.7+-blue.svg)](https://www.python.org/downloads/)

## 🚀 Installation

```bash
pip install numcore
```

## 📖 Usage

### **Statistical Analysis**
```python
from numcore import mean, median, mode, std, analyze_list

data = [23, 45, 67, 45, 89, 34, 78, 98, 54, 55]
print(mean(data))      # 58.8
print(median(data))    # 54.5
analysis = analyze_list(data)
print(analysis['variance'])
```

### **Number Theory**
```python
from numcore import (factorial, is_prime, gcd, prime_factorization,
                     euler_totient, mobius, legendre_symbol)

print(factorial(5))              # 120
print(is_prime(17))             # True
print(gcd(48, 18))              # 6
print(prime_factorization(100)) # [2, 2, 5, 5]
print(euler_totient(9))         # 6
print(mobius(30))               # -1
print(legendre_symbol(2, 7))    # 1
```

### **Sequences**
```python
from numcore import (fibonacci, arithmetic_seq, geometric_seq, 
                     lucas, collatz, farey)

print(fibonacci(10))            # [0, 1, 1, 2, 3, 5, 8, 13, 21, 34]
print(arithmetic_seq(2, 3, 5))  # [2, 5, 8, 11, 14]
print(geometric_seq(2, 3, 4))   # [2, 6, 18, 54]
print(lucas(7))                 # [2, 1, 3, 4, 7, 11, 18]
print(collatz(10))              # [10, 5, 16, 8, 4, 2, 1]
print(farey(4))                 # [(0,1), (1,4), (1,3), (1,2), (2,3), (3,4), (1,1)]
```

### **Combinatorics**
```python
from numcore import npr, ncr

print(npr(5, 3))  # 60  - Permutations
print(ncr(5, 3))  # 10  - Combinations
```

### **Matrix Operations**
```python
from numcore import (create_matrix, matrix_multiply, determinant, 
                     matrix_transpose, matrix_power)

mat = [[1, 2], [3, 4]]
print(determinant(mat))          # -2
print(matrix_transpose(mat))     # [[1, 3], [2, 4]]
print(matrix_power(mat, 2))      # [[7, 10], [15, 22]]
```

## ✨ Features

### **Input Functions**
- `n_input(n)` - Get n integers from user with validation

### **List Utilities**
- `counter(lst)` - Count occurrences of items
- `product(lst)` - Multiply all numbers
- `power_list(lst, power)` - Apply power to each element

### **Statistical Functions**
- `mean(lst)` - Calculate average
- `median(lst)` - Find middle value
- `mode(lst)` - Find most common value(s)
- `variance(lst, sample=False)` - Calculate variance
- `std(lst, sample=False)` - Calculate standard deviation
- `analyze_list(lst)` - Comprehensive statistical analysis

### **Number Theory**
- `factorial(n)` - Calculate n!
- `nth_root(num, n)` - Calculate nth root
- `divisors(num)` - Find all divisors
- `proper_divisors(num)` - Divisors excluding number itself
- `common_divisors(num1, num2)` - Common divisors
- `gcd(num1, num2)` - Greatest common divisor
- `lcm(num1, num2)` - Least common multiple
- `is_prime(num)` - Check if prime
- `primes(num)` - All primes up to num
- `prime_divisors(num)` - Prime divisors only
- `prime_factorization(num)` - Prime factorization
- `prime_factors(num)` - Unique prime factors
- `is_perfect(num)` - Check if perfect number
- `is_armstrong(num)` - Check if Armstrong number
- `is_amicable(a, b)` - Check if amicable pair
- `euler_totient(num)` - Euler's φ function
- `mobius(num)` - Möbius function μ(n)
- `quadratic_residue(num)` - Quadratic residues mod n
- `quadratic_non_residue(num)` - Quadratic non-residues mod n
- `legendre_symbol(a, p)` - Legendre symbol (a/p)

### **Sequences**
- `fibonacci(num)` - Fibonacci sequence
- `nth_fibonacci(num)` - nth Fibonacci number
- `lucas(num)` - Lucas sequence
- `nth_lucas(num)` - nth Lucas number
- `arithmetic_seq(a, d, n)` - Arithmetic sequence
- `nth_arithmetic(a, d, n)` - nth term of AP
- `arithmetic_sum(a, d, n)` - Sum of AP
- `geometric_seq(a, r, n)` - Geometric sequence
- `nth_geometric(a, r, n)` - nth term of GP
- `geometric_sum(a, r, n)` - Sum of GP
- `harmonic_seq(a, d, n)` - Harmonic sequence
- `nth_harmonic(a, d, n)` - nth harmonic term
- `harmonic_sum(a, d, n)` - Sum of harmonic sequence
- `collatz(n)` - Collatz sequence (3n+1 problem)
- `farey(num)` - Farey sequence of order n

### **Combinatorics**
- `npr(n, r)` - Permutations nPr
- `ncr(n, r)` - Combinations nCr

### **Digit Operations**
- `digits(num)` - Extract digits as list
- `reverse_number(num)` - Reverse digits
- `sum_of_digits(num)` - Sum all digits

### **Basic Matrix Operations**
- `create_matrix(rows, cols, fill=0)` - Create matrix
- `input_matrix()` - Interactive input
- `matrix_shape(matrix)` - Get dimensions
- `matrix_add(mat1, mat2)` - Matrix addition
- `matrix_sub(mat1, mat2)` - Matrix subtraction
- `scalar_multiply(matrix, scalar)` - Scalar multiplication
- `matrix_multiply(mat1, mat2)` - Matrix multiplication

### **Advanced Matrix Operations**
- `matrix_identity(rows)` - Identity matrix
- `matrix_transpose(matrix)` - Transpose
- `matrix_trace(matrix)` - Trace (sum of diagonal)
- `determinant(matrix)` - Determinant (recursive)
- `matrix_minor(matrix)` - Matrix of minors
- `matrix_cofactor(matrix)` - Cofactor matrix
- `matrix_power(matrix, power)` - Matrix exponentiation
- `is_square(matrix)` - Check if square
- `is_orthogonal(matrix)` - Check if orthogonal

## 🎯 Roadmap

- [x] Basic input functions (v0.1.0)
- [x] List utilities (v0.1.2)
- [x] Statistical functions (v0.1.3)
- [x] Number theory basics (v0.1.4)
- [x] Basic matrix operations (v0.1.5)
- [x] Advanced matrix operations (v0.1.6)
- [x] Sequences & digit operations (v0.1.7)
- [x] Advanced number theory & combinatorics (v0.1.8)
- [ ] Trigonometry functions
- [ ] Matrix decomposition (LU, QR, eigenvalues)
- [ ] Algebra (solve equations, polynomials)
- [ ] Calculus (derivatives, integrals)
- [ ] Advanced statistics (correlation, regression)
- [ ] **Goal: 250+ functions!**

## 📊 Progress

**Current Functions:** 67/250 (26.8%)

## 💡 Example Use Cases

### **Collatz Conjecture**
```python
from numcore import collatz

# Test the famous 3n+1 problem
sequence = collatz(27)
print(f"Steps: {len(sequence)}")  # 111 steps!
```

### **Euler's Totient in Cryptography**
```python
from numcore import euler_totient

# Used in RSA encryption
phi_n = euler_totient(15)  # 8
# Numbers coprime to 15: 1,2,4,7,8,11,13,14
```

### **Farey Sequence (Continued Fractions)**
```python
from numcore import farey

# All fractions between 0 and 1
fractions = farey(5)
# [(0,1), (1,5), (1,4), (1,3), (2,5), (1,2), ...]
```

### **Legendre Symbol (Quadratic Residues)**
```python
from numcore import legendre_symbol

# Check if 2 is a quadratic residue modulo 7
result = legendre_symbol(2, 7)  # 1 (yes!)
# Because 3² ≡ 9 ≡ 2 (mod 7)
```

## 🛠️ Development

### **Requirements**
- Python 3.7+
- No external dependencies!

### **Testing**
```python
# Example test
from numcore import ncr, npr
assert ncr(5, 3) == 10
assert npr(5, 3) == 60
```

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

Built by a first-year student, documenting the journey from basic Python to advanced mathematical algorithms.

### **Milestones**
- ✅ Published to PyPI
- ✅ 67 functions implemented
- ✅ Recursive determinant calculation
- ✅ Complete sequence generation suite
- ✅ Advanced number theory (Möbius, Euler's φ, Legendre)
- ✅ **Reached 26.8% (over 1/4 complete!)**
- 🎯 Next: 100 functions (40%)

### **Why numcore?**
- Learn by building from scratch
- Pure Python (no dependencies)
- Comprehensive documentation
- Open source learning resource

## 📚 Function Categories

| Category | Functions | Completion |
|----------|-----------|------------|
| Statistics | 6 | ✅ |
| Number Theory | 22 | 🔄 Growing |
| Sequences | 15 | 🔄 Growing |
| Combinatorics | 2 | 🔄 Growing |
| Digit Ops | 3 | ✅ |
| Matrix Basic | 7 | ✅ |
| Matrix Advanced | 9 | ✅ |
| List Utils | 3 | 🔄 Growing |
| **Total** | **67** | **26.8%** |

---

Crafted with Python. Powered by curiosity. Open-sourced for learning. ⚡