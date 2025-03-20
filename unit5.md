### 📌 Python Packages Notes  

#### 🔹 **Python Package Kya Hota Hai?**  
Python me **package ek folder hota hai jo multiple modules ko contain karta hai**.

- **Module** ek single Python file hoti hai (`.py` extension ke saath).
- **Package** ek folder hota hai jo multiple modules ko contain karta hai.
- **Har package me ek special file `__init__.py` hoti hai**, jo Python ko batati hai ki yeh ek package hai.

---

## 🔹 **Python Package Structure**
```bash
mypackage/          # Main package folder
│
├── __init__.py    # Required file to make this a package
├── mod1.py        # First module
├── mod2.py        # Second module
└── subpackage/    # Sub-package inside main package
    ├── __init__.py
    ├── submod1.py
    └── submod2.py
```

📌 **Explanation:**
- `mypackage` ek package hai.
- `__init__.py` file har package me hoti hai jo usko ek **valid Python package** banati hai.
- `mod1.py`, `mod2.py` alag-alag modules hain jo `mypackage` me hain.
- `subpackage/` ek nested package hai jo aur modules contain karta hai.

---

## ✅ **Python Package Import Karne Ke Tarike**

### ➤ **1. Direct Import Using `import`**
```python
import mypackage.mod1
mypackage.mod1.function_name()
```
📌 **Explanation:**
- Pura package import karne ke baad `mod1` ke function ko call kar sakte hain.

### ➤ **2. Import Specific Function From Module**
```python
from mypackage.mod1 import function_name
function_name()
```
📌 **Explanation:**
- Sirf ek specific function ko import kiya ja sakta hai jo module me hai.

### ➤ **3. Importing Everything From a Module (`*`)**
```python
from mypackage.mod1 import *
```
📌 **Explanation:**
- Is tarah se module ke **sare functions/classes import** kiye ja sakte hain.

### ➤ **4. Importing a Subpackage**
```python
from mypackage.subpackage.submod1 import sub_function
sub_function()
```
📌 **Explanation:**
- Agar package ke andar ek **subpackage** hai, to usko bhi import kar sakte hain.

---

## ✅ **Example Code (`mypackage/mod1.py`)**
```python
# mypackage/mod1.py

def greet(name):
    return f"Hello, {name}!"
```

### **Main File (`main.py`)**
```python
from mypackage.mod1 import greet

print(greet("Python User"))
```
📌 **Explanation:**
- `greet` function `mod1.py` me hai aur `main.py` me usko import kiya.
- `main.py` run karne par output aayega: `Hello, Python User!`

---

### ✅ **Key Points:**
1. **Package ek folder hota hai jo multiple modules contain karta hai.**
2. **`__init__.py` package ko define karta hai aur required hota hai.**
3. **Alag-alag tariko se import kiya ja sakta hai (`import`, `from ... import`, `*`).**
4. **Nested sub-packages bhi support hote hain.**

---

