# Stack in Python

This project implements a Stack (LIFO - Last In, First Out) in Python with basic operations:  
- Push values  
- Pop values  
- Check if the stack is empty (`is_empty`)  
- Get the top value (`get_top`)  
- Get stack size (`len(stack)`)  
- String representation of the stack  

---

## 🐍 1. Basic Usage (easiest way)

If you just want to try the stack without installing anything, copy **`stack.py`** into the same folder as your project and use:

```python
from stack import Stack

s = Stack()
s.push(1)
s.push(2)
s.push(3)
print(s.get_top())  # 3
print(len(s))       # 3
```

---

## 📦 2. Advanced Usage (install as a package)

If you want to use this as a Python package, you first need **Git installed**.  
👉 [Download Git](https://git-scm.com/downloads) if you don’t already have it.

Then install directly from GitHub using pip:

```bash
pip install git+https://github.com/Ahmedhm1/Stack-python.git
```

Now you can import it anywhere:

```python
from stk import Stack

s = Stack()
s.push(10)
s.push(20)
print(s.get_top())  # 20
```

---

## 🔎 Example Usage

```python
from stk import Stack

s = Stack()

# Push values
s.push(5)
s.push(8)
s.push(12)

# Pop a value
s.pop()  # removes 12

# Get top value
print(s.get_top())  # 8

# Check if empty
print(s.is_empty())  # False

# Print stack
print(s)
```

---

## 📂 Project Structure
```
Stack-python/
│
├── stk/            # Package source code
│   ├── __init__.py   # Exports Stack
│   └── stack.py      # Stack implementation
│
├── README.md
├── pyproject.toml    # modern build file
└── setup.py          # Package setup script
```

---

## 📖 Source Code
➡️ [View `stack.py`](./stk/stack.py) directly if you just want to read the implementation.
