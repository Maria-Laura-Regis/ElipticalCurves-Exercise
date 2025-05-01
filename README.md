# Elliptic Curve Point Generation

This C++ program demonstrates the generation of points on an elliptic curve by computing scalar multiples of a given generator point.

## 📌 Program Overview

Implements elliptic curve arithmetic over a finite field 𝔽ₚ with:
- Point addition/doubling operations
- Modular inverse calculation
- Curve membership verification

## 🛠️ Technical Details

### Curve Parameters
- **Equation**: y² ≡ x³ + 2x + 2 (mod 17)
- **Generator Point (G)**: (5, 1)
- **Prime Modulus (p)**: 17
- **Point at Infinity (O)**: Represented as (INT_MAX, INT_MAX)


### The program ilustrates:
⟨G⟩ = {nG | n ∈ ℤ⁺} forms a finite cyclic subgroup


### Core Functions

```c
int is_on_curve(Point p, int a, int b, int p_mod)  // Verify point lies on curve
int inv_mod(int a, int p)                         // Modular inverse (naive implementation)
Point point_add(Point P, Point Q, int a, int p)   // Point addition/doubling
```
