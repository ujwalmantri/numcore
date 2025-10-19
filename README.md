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

# Basic statistics
print(mean(data))      # 58.8
print(median(data))    # 54.5
print(mode(data))      # [45]
print(std(data))       # 23.82

# Comprehensive analysis
analysis = analyze_list(data)
print(analysis['mean'])
print(analysis['variance'])
print(analysis['frequency'])
```

### **Number Theory**
```python
from numcore import factorial, is_prime, gcd, lcm, prime_factorization

print(factorial(5))              # 120
print(is_prime(17))             # True
print(gcd(48, 18))              # 6
print(lcm(12, 18))              # 36
print(prime_factorization(100)) # [2, 2, 5, 5]
print(divisors(24))             # [1, 2, 3, 4, 6, 8, 12, 24]
```

### **Matrix Operations**
```python
from numcore import create_matrix, matrix_add, matrix_multiply, scalar_multiply

# Create matrices
mat1 = create_matrix(2, 2, fill=1)  # [[1, 1], [1, 1]]
mat2 = [[2, 3], [4, 5]]

# Matrix operations
sum_mat = matrix_add(mat1, mat2)         # [[3, 4], [5, 6]]
product = matrix_multiply(mat1, mat2)    # [[6, 8], [6, 8]]
scaled = scalar_multiply(mat2, 3)        # [[6, 9], [12, 15]]

# Get matrix dimensions
rows, cols = matrix_shape(mat1)  # (2, 2)
```

## ✨ Features

### **Input Functions**
- `n_input(n)` - Get n integers from user with validation

### **List Utilities**
- `counter(lst)` - Count occurrences of items in a list
- `product(lst)` - Multiply all numbers in a list

### **Statistical Functions**
- `mean(lst)` - Calculate average
- `median(lst)` - Find middle value
- `mode(lst)` - Find most common value(s)
- `variance(lst, sample=False)` - Calculate variance (population or sample)
- `std(lst, sample=False)` - Calculate standard deviation
- `analyze_list(lst)` - Comprehensive statistical analysis with mean, median, mode, variance, std, frequency, and more

### **Number Theory**
- `factorial(n)` - Calculate n! (factorial)
- `nth_root(num, n)` - Calculate nth root of a number
- `divisors(num)` - Find all divisors of a number (optimized algorithm)
- `common_divisors(num1, num2)` - Find common divisors of two numbers
- `gcd(num1, num2)` - Greatest common divisor (Euclidean algorithm)
- `lcm(num1, num2)` - Least common multiple
- `is_prime(num)` - Check if a number is prime (optimized)
- `primes(num)` - Get all prime numbers up to num
- `prime_divisors(num)` - Find prime divisors of a number
- `prime_factorization(num)` - Prime factorization with repetition
- `prime_factors(num)` - Unique prime factors
- `is_perfect(num)` - Check if number is perfect (sum of divisors equals number)

### **Matrix Operations**
- `create_matrix(rows, cols, fill=0)` - Create m×n matrix filled with a value
- `input_matrix()` - Interactive matrix input from user
- `matrix_shape(matrix)` - Get dimensions and validate matrix structure
- `matrix_add(mat1, mat2)` - Add two matrices element-wise
- `matrix_sub(mat1, mat2)` - Subtract two matrices element-wise
- `scalar_multiply(matrix, scalar)` - Multiply matrix by a scalar
- `matrix_multiply(mat1, mat2)` - Matrix multiplication (dot product)

## 🎯 Roadmap

- [x] Basic input functions (v0.1.0)
- [x] List utilities (v0.1.2)
- [x] Statistical functions (v0.1.3)
- [x] Number theory functions (v0.1.4)
- [x] Matrix operations (v0.1.5)
- [ ] Trigonometry functions (sin, cos, tan with degrees)
- [ ] Advanced matrix operations (transpose, determinant, inverse)
- [ ] Algebra functions (solve equations, quadratic formula)
- [ ] Calculus functions (derivatives, integrals)
- [ ] More advanced statistics (correlation, regression)
- [ ] **Goal: 250+ functions!**

## 📊 Progress

**Current Functions:** 28/250 (11.2%)

## 💡 Example Use Cases

### **Analyzing Test Scores**
```python
from numcore import analyze_list

scores = [85, 92, 78, 90, 88, 76, 95, 89, 84, 91]
analysis = analyze_list(scores)

print(f"Average: {analysis['mean']}")
print(f"Median: {analysis['median']}")
print(f"Std Dev: {analysis['std']['population std']}")
```

### **Finding Prime Factors**
```python
from numcore import prime_factorization, prime_factors

number = 360
print(f"Prime factorization: {prime_factorization(number)}")  # [2, 2, 2, 3, 3, 5]
print(f"Unique prime factors: {prime_factors(number)}")       # [2, 3, 5]
```

### **Matrix Transformations**
```python
from numcore import create_matrix, matrix_multiply, scalar_multiply

# Create transformation matrix
transform = [[2, 0], [0, 2]]  # Scale by 2

# Apply to vector
point = [[1], [3]]
result = matrix_multiply(transform, point)  # [[2], [6]]
```

## 🛠️ Development

### **Requirements**
- Python 3.7+
- No external dependencies!

### **Contributing**
This is a learning project, but suggestions and feedback are welcome! Feel free to:
- Report bugs via GitHub Issues
- Suggest new functions
- Share how you're using numcore

## 📝 License

MIT License - see [LICENSE](LICENSE) file for details

## 👨‍💻 Author

**Ujwal Mantri**
- PyPI: [numcore](https://pypi.org/project/numcore/)
- GitHub: [ujwalmantri](https://github.com/ujwalmantri/numcore)
- Email: ujwalmantrifr@gmail.com

## 🌟 Support

If you find this helpful, please:
- ⭐ Star the repository on GitHub
- 📦 Try it out: `pip install numcore`
- 📢 Share with others learning Python

## 🎓 Learning Journey

This library is being built as a learning project by a first-year student. It documents the journey from basic Python concepts to advanced mathematical algorithms. Each function is implemented from scratch to maximize learning.

### **Why numcore?**
- ✅ Learn by building
- ✅ No dependencies - pure Python
- ✅ Well-documented with examples
- ✅ Growing collection of useful functions
- ✅ Open source for everyone to learn from

---

Crafted with Python. Powered by curiosity. Open-sourced for learning. ⚡