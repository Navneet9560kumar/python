📚 Python Lecture 2 Notes - Mutable vs Immutable


🔍 Mutable and Immutable Objects in Python

✅ What are Immutable Objects?
.Definition: Immutable objects are those that cannot be changed after their creation.

.Examples: int, float, str, tuple, frozenset.

.Memory Management:

   .When you try to modify an immutable object, a new object is created instead of changing the original one.
   .This leads to memory efficiency in some cases, as multiple variables can point to the same object in memory (interning).
   x = 10
   y = x
   x = 20
  print(y)  # Output: 10 (y does not change with x)

⚙️ What are Mutable Objects?
  .Definition: Mutable objects are those that can be modified after creation.

   .Examples: list, dict, set.

  .Memory Management:
   .Mutable objects can be changed without creating a new object. Their memory location remains the same but their content can change.
   .This allows efficient in-place modification.

lst = [1, 2, 3]
lst2 = lst
lst[0] = 10
print(lst2)  # Output: [10, 2, 3] (lst and lst2 point to the same object)




I see! Here's the entire Python Lecture 2 Notes in one block so you can easily copy and paste it into your file:

📚 Python Lecture 2 Notes - Mutable vs Immutable
🔍 Mutable and Immutable Objects in Python
✅ What are Immutable Objects?
Definition: Immutable objects are those that cannot be changed after their creation.

Examples: int, float, str, tuple, frozenset.

Memory Management:

When you try to modify an immutable object, a new object is created instead of changing the original one.
This leads to memory efficiency in some cases, as multiple variables can point to the same object in memory (interning).
Example:

python
Copy
Edit
x = 10
y = x
x = 20
print(y)  # Output: 10 (y does not change with x)
⚙️ What are Mutable Objects?
Definition: Mutable objects are those that can be modified after creation.

Examples: list, dict, set.

Memory Management:

Mutable objects can be changed without creating a new object. Their memory location remains the same but their content can change.
This allows efficient in-place modification.
Example:

python
Copy
Edit
lst = [1, 2, 3]
lst2 = lst
lst[0] = 10
print(lst2)  # Output: [10, 2, 3] (lst and lst2 point to the same object)



   🔄 How Python Handles Memory for Mutable vs Immutable Objects
  

Python reuses the same memory location for identical values. If an object is modified, a new one is created at a different location.

Mutable Objects:
Memory address remains the same even after modifications. This is efficient for scenarios where data changes often.

