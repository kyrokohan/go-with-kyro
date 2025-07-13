# 02 – FizzBuzz Variants

Build classic *FizzBuzz* (and a few twists) to practice loops and conditionals.

**Difficulty:** Fundamentals (≈15 min)

---

## 🎯 Learning objectives

- Use `for` loops for iteration
- Implement conditional logic with modulo operations
- Parse integer command-line flags with Go’s `flag` package

---

## 🌟 Required goals

| # | Requirement | Quick check |
|---|-------------|-------------|
| 1 | Print numbers **1–100**, replacing multiples of **3** with `Fizz`, multiples of **5** with `Buzz`, and multiples of both with `FizzBuzz`. | `go run .` → `… 14 FizzBuzz 16 … 98 Fizz 99 Buzz 100` |
| 2 | Accept a **`--max`** flag (long form only) to choose the upper bound (default **100**). | `go run . --max 20` → output ends at `20` | 