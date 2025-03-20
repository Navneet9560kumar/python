### 📌 Python Dictionary Notes  

#### 🔹 **Dictionary Kya Hai?**  
Python **Dictionary** ek unordered collection hoti hai jo **key-value pairs** me data store karti hai. Isme har key unique hoti hai aur uske corresponding ek value hoti hai. Yeh **mutable** hoti hai, yani hum dictionary ko modify kar sakte hain.  

#### 🔹 **Dictionary Banane Ka Tarika**  
```python
# Empty dictionary
my_dict = {}

# Dictionary with values
student = {
    "name": "Rahul",
    "age": 20,
    "marks": 85.5
}

# Mixed data types
info = {
    "name": "Priya",
    "age": 25,
    "hobbies": ["reading", "coding"],
    "is_student": False
}
```

#### 🔹 **Dictionary Access Karna**  
```python
student = {"name": "Rahul", "age": 20, "marks": 85.5}

# Accessing values using keys
print(student["name"])  # Rahul
print(student.get("age"))  # 20

# Accessing a key that may not exist (safe way)
print(student.get("city", "Not Found"))  # Not Found
```

#### 🔹 **Dictionary Methods (Common Operations)**  
```python
student = {"name": "Rahul", "age": 20, "marks": 85.5}

# Adding new key-value pair
student["city"] = "Delhi"

# Updating an existing value
student["age"] = 21

# Removing a key-value pair
del student["marks"]

# Using pop method
gender = student.pop("gender", "Not Found")  # Returns default if key not found

# Getting all keys and values
print(student.keys())  # dict_keys(["name", "age", "city"])
print(student.values())  # dict_values(["Rahul", 21, "Delhi"])
print(student.items())  # dict_items([(key, value), (key, value)])

# Checking if a key exists
print("name" in student)  # True
```

#### 🔹 **Dictionary Iteration**  
```python
student = {"name": "Rahul", "age": 20, "city": "Delhi"}

# Iterating over keys
for key in student:
    print(key, "->", student[key])

# Iterating over key-value pairs
for key, value in student.items():
    print(f"{key}: {value}")
```

#### 🔹 **Nested Dictionary (Dictionary ke andar Dictionary)**
```python
students = {
    "student1": {"name": "Amit", "age": 22},
    "student2": {"name": "Neha", "age": 21}
}

# Accessing nested values
print(students["student1"]["name"])  # Amit
print(students["student2"]["age"])  # 21
```

#### 🔹 **Dictionary Comprehension (Shorter Syntax for Creating Dictionaries)**
```python
# Creating a dictionary with squares
squares = {x: x**2 for x in range(1, 6)}
print(squares)  # {1: 1, 2: 4, 3: 9, 4: 16, 5: 25}
```

---
### ✅ **Key Points:**
1. Dictionary **key-value pairs** me data store karta hai.
2. **Keys unique** hoti hain, values same ho sakti hain.
3. Dictionary **mutable** hoti hai, yani modify kar sakte hain.
4. Dictionary **unordered** hoti hai, yani indexing nahi hoti.
5. `.get()` method safe hota hai unknown keys access karne ke liye.
6. `.keys()`, `.values()`, aur `.items()` methods dictionary ko explore karne ke liye useful hain.
7. **Nested dictionaries** aur **dictionary comprehension** ka use bhi hota hai.

---

