# 03 – Calculator REPL

Build an interactive command-line calculator to practice loops, input parsing, and basic arithmetic in Go.

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

---

## 🚀 Stretch goals (optional)

1. Support **parentheses** and standard operator precedence (`2 * (3 + 4)` → `14`).
2. Accept **floating-point numbers** and print results with reasonable precision.
3. Remember the **last result** in a variable (e.g., `_`) that can be reused in the next expression.
4. Add a **`--prompt`** flag to customize the prompt string (`go run . --prompt "$ "`).
5. Provide a **help** command (`help`) that lists the supported operators and commands.
6. Write table-driven unit tests for the expression evaluator (`go test`). 