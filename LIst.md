### 📌 Python List Notes  

#### 🔹 **List Kya Hai?**  
Python **List** ek ordered collection hoti hai jisme multiple values store kar sakte hain. Yeh **mutable** hoti hai, yani iski values ko change kiya ja sakta hai. List me **different data types** bhi store kar sakte hain.  

#### 🔹 **List Banane Ka Tarika**  
```python
# Empty list
my_list = []

# List with values
numbers = [1, 2, 3, 4, 5]
fruits = ["apple", "banana", "mango"]
mixed = [1, "hello", 3.5, True]  # Different data types allowed
```

#### 🔹 **List Indexing & Slicing**  
```python
fruits = ["apple", "banana", "mango", "orange"]

# Accessing elements using index (0-based indexing)
print(fruits[0])  # apple
print(fruits[2])  # mango

# Negative Indexing
print(fruits[-1])  # orange (last element)
print(fruits[-2])  # mango (second last element)

# Slicing
print(fruits[1:3])  # ['banana', 'mango']
print(fruits[:2])   # ['apple', 'banana']
print(fruits[2:])   # ['mango', 'orange']
print(fruits[-3:-1])  # ['banana', 'mango']
```

#### 🔹 **List Methods (Common Operations)**  
```python
numbers = [10, 20, 30, 40]

# Add elements
numbers.append(50)   # [10, 20, 30, 40, 50]
numbers.insert(2, 25)  # [10, 20, 25, 30, 40, 50]

# Remove elements
numbers.remove(30)  # [10, 20, 25, 40, 50]
popped = numbers.pop()  # Removes last element and returns it
print(popped)  # 50

# Finding index
print(numbers.index(25))  # 2

# Count occurrences of an element
print(numbers.count(20))  # 1

# Sorting and reversing
numbers.sort()  # Ascending order
numbers.reverse()  # Reverse the list

# Copying a list
new_list = numbers.copy()

# Clearing a list
numbers.clear()
```

#### 🔹 **List Comprehension (Shorter Syntax for Creating Lists)**
```python
# Creating a list with a loop
squares = [x**2 for x in range(1, 6)]
print(squares)  # [1, 4, 9, 16, 25]

# Filtering in list comprehension
evens = [x for x in range(10) if x % 2 == 0]
print(evens)  # [0, 2, 4, 6, 8]
```

#### 🔹 **Nested Lists (List Inside a List)**
```python
matrix = [[1, 2, 3], [4, 5, 6], [7, 8, 9]]

# Accessing elements
print(matrix[0])  # [1, 2, 3]
print(matrix[1][1])  # 5
```

#### 🔹 **List Iteration**
```python
numbers = [1, 2, 3, 4, 5]

# Using for loop
for num in numbers:
    print(num)

# Using while loop
i = 0
while i < len(numbers):
    print(numbers[i])
    i += 1
```

---
### ✅ **Key Points:**
1. List is **ordered** and **mutable**.
2. Supports **indexing** and **slicing**.
3. Can contain **different data types**.
4. Provides **built-in methods** for modification.
5. Supports **list comprehension** for concise syntax.
6. Allows **nested lists** for complex structures.

---

