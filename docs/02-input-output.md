### EXAMINE INPUT AND OUTPUT IN THE LINUX SHELL 

As a security professional, it’s important to understand how to interact with your computer through the shell. In this tutorial, you will learn how to:

* Generate output using the `echo` command.
* Perform simple calculations using the `expr` command.
* Clear the shell window with the `clear` command.

---

## 1. Generate Output with the `echo` Command

The `echo` command outputs a specified string of text to the shell.

### Example 1: Simple Text Output

```bash
echo hello
```

**Output:**

```
hello
```

### Example 2: Output with Quotation Marks

```bash
echo "MyName"
```

**Output:**

```
MyName
```

📌 *Quotation marks are optional, but they group characters together. This is useful when working with strings that contain spaces or special characters.*

---

## 2. Perform Calculations with the `expr` Command

The `expr` command allows you to perform basic mathematical operations.

### Example 1: Subtraction

If you received **32 alerts** and only **8 require action**, calculate the number of false positives:

```bash
expr 32 - 8
```

**Output:**

```
24
```

### Important Notes:

* **Spaces are required** between numbers and operators.

  * ✅ `expr 32 - 8`
  * ❌ `expr 32-8`
* Operators supported: `+`, `-`, `/`, `*`
* Only **integer math** is supported (no decimals).

---

## 3. Clear the Shell

To clear previous commands and outputs:

```bash
clear
```

This resets the terminal screen and places the cursor at the top, creating a clutter-free workspace.

---

✅ **Key Takeaways**

* `echo` outputs text or strings to the shell.
* `expr` performs basic integer arithmetic.
* `clear` removes all previous outputs for a clean terminal view.

---
