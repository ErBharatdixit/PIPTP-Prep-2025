# 🔁 Recursive Pattern Generator

## 📘 Problem Statement

Write a recursive function `f(n)` with one positive integer parameter `n`.

The function prints **`2^n - 1` integers** in the following specific pattern:

### 🧾 Example Outputs

```txt
f(1) → 1

f(2) → 1 2 1

f(3) → 1 2 1 3 1 2 1

f(4) → 1 2 1 3 1 2 1 4 1 2 1 3 1 2 1

f(5) → 1 2 1 3 1 2 1 4 1 2 1 3 1 2 1 5 1 2 1 3 1 2 1 4 1 2 1 3 1 2 1


---

## 💡 Recursive Pattern Logic

At each level `n`, the output pattern is constructed as:

```text
f(n) = f(n - 1), print(n), f(n - 1)

                f(3)
             /   |   \
          f(2)   3   f(2)
        /  |  \      / |  \
     f(1) 2 f(1)  f(1) 2 f(1)

Output: 1 2 1 3 1 2 1

## Time Complexity O(2^n-1)

