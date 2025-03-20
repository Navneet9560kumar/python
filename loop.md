### 📌 Python Loops Notes  

#### 🔹 **Loops Kya Hain?**  
Loops ka use **repetitive tasks** ko automate karne ke liye hota hai. Python me **for loop** aur **while loop** ka use kiya jata hai.

---

## 🔹 **Types of Loops in Python**
1. **for loop**
2. **while loop**
3. **Nested loops**
4. **Loop control statements (break, continue, pass)**

---

## ✅ **Question 1: Count Positive Numbers**
```python
numbers = [1, -2, 3, -4, 5, 6, -7, -8, 9, 10]
pos = 0

for num in numbers:
    if num > 0:
        pos += 1

print("Count of positive numbers:", pos)
```
📌 **Explanation:**
- List ke andar jitne positive numbers hain, unka count find kar raha hai.
- Loop har element check karega aur agar positive hai to counter badh jayega.

---

## ✅ **Question 2: Count Even Numbers**
```python
numbers = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10]
even_count = 0

for num in numbers:
    if num % 2 == 0:
        even_count += 1

print("Count of even numbers:", even_count)
```
📌 **Explanation:**
- List ke andar jitne **even numbers** hain, unka count find kar raha hai.
- Agar number `2` se divide hone par remainder `0` aata hai to woh **even** hai.

---

## ✅ **Question 3: Print Table (Skipping 5th Iteration)**
```python
number = 7

for i in range(1, 11):
    if i == 5:
        continue  # Skip 5th iteration
    print(number, 'x', i, '=', number * i)
```
📌 **Explanation:**
- Yeh loop **7 ka table** print karega.
- **5th iteration ko skip** karne ke liye `continue` statement use kiya gaya hai.

---

## ✅ **Question 4: Reverse a String**
```python
input_str = 'Python'
reverse_str = ""

for char in input_str:
    reverse_str = char + reverse_str

print("Reversed String:", reverse_str)
```
📌 **Explanation:**
- Har character ko pehle se reverse_str me add karte jayenge.
- Isse string **reverse** ho jayegi.

---

## ✅ **Question 5: Find the First Non-Repeated Character**
```python
input_str = "aabbcdeff"

for char in input_str:
    if input_str.count(char) == 1:  # Character ek hi baar aaya ho
        print("First Non-Repeated Character:", char)
        break
```
📌 **Explanation:**
- `count(char)` function character ka occurrence check karega.
- Jo pehla **non-repeating character** milega, usko print karke loop break kar denge.

---

## ✅ **Question 6: Factorial Calculator (Using While Loop)**
```python
number = 5
factorial = 1

while number > 0:
    factorial *= number  # Multiplication
    number -= 1  # Decrement

print("Factorial:", factorial)
```
📌 **Explanation:**
- `while` loop tab tak chalega jab tak `number` zero nahi ho jata.
- **Factorial calculation** ke liye multiplication aur decrement ho raha hai.

---

## ✅ **Question 7: Check Prime Number**
```python
num = 29
is_prime = True

if num > 1:
    for i in range(2, int(num ** 0.5) + 1):
        if num % i == 0:
            is_prime = False
            break

print(num, "is Prime" if is_prime else "is Not Prime")
```
📌 **Explanation:**
- **Prime number wahi hota hai jo sirf 1 aur khud se divisible ho.**
- `range(2, sqrt(n))` tak loop chalayenge kyunki kisi number ka **factor sqrt(n) tak hi hota hai**.

---

## ✅ **Extra Questions for Practice**

### ➤ **Question 8: Print Fibonacci Series (Up to N terms)**
```python
n = 10  # Number of terms
fib1, fib2 = 0, 1

print(fib1, fib2, end=' ')
for _ in range(n - 2):
    fib_next = fib1 + fib2
    print(fib_next, end=' ')
    fib1, fib2 = fib2, fib_next
```
📌 **Explanation:**
- Fibonacci series ka rule: `F(n) = F(n-1) + F(n-2)`
- Pehle do terms fix hoti hain (0,1) aur agli terms previous do ka sum hoti hain.

---

### ➤ **Question 9: Sum of Digits of a Number**
```python
num = 12345
sum_digits = 0

while num > 0:
    sum_digits += num % 10  # Extract last digit and add
    num //= 10  # Remove last digit

print("Sum of digits:", sum_digits)
```
📌 **Explanation:**
- Har iteration me last digit extract karte hain (`num % 10`) aur `sum_digits` me add kar dete hain.
- `num //= 10` se last digit remove hoti hai.

---

### ➤ **Question 10: Find Largest Number in a List**
```python
numbers = [5, 10, 25, 7, 30, 14]
largest = numbers[0]

for num in numbers:
    if num > largest:
        largest = num

print("Largest Number:", largest)
```
📌 **Explanation:**
- Pehla element `largest` maana.
- Loop chalakar har number ko check kiya ki kya woh `largest` se bada hai.

---

### ✅ **Key Points:**
1. **for loop** ka use jab pata ho kitni baar loop chalana hai.
2. **while loop** ka use jab condition satisfy hone tak loop chalana ho.
3. **break, continue, pass** statements loop control ke liye use hote hain.
4. **Nested loops** ka use jab ek loop ke andar doosra loop ho.

---

