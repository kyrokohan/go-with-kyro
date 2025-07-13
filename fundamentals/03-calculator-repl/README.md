# 03 – Calculator REPL

Build an interactive command-line calculator to practice loops, input parsing, and basic arithmetic in Go.

**Difficulty:** Fundamentals (≈25 min)

---

## 🎯 Learning objectives

- Build a read–eval–print loop (REPL)
- Parse and evaluate basic arithmetic expressions
- Handle user input errors gracefully

---

## 🌟 Required goals

| # | Requirement | Quick check |
|---|-------------|-------------|
| 1 | Launch a **read–eval–print loop (REPL)** that repeatedly prompts `>` for input until the user types **`exit`** or **`quit`**. | `go run .` → displays `>` prompt |
| 2 | Parse and evaluate single-line expressions containing two integers and an operator `+`, `-`, `*`, or `/` (integer division). | `> 7 * 8` → `56` |
| 3 | Ignore surrounding whitespace in expressions. | `>  12  /3 ` → `4` |
| 4 | Print `error: <message>` for invalid input instead of crashing, then continue the loop. | `> hello` → `error: invalid expression` |

Keep the implementation simple and focused on correct parsing and looping.

You do **not** need a full tokenizer—splitting the input into `<int> <op> <int>` (e.g., via `strings.Fields` or `fmt.Sscanf`) is enough for the required goals. 