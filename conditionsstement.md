### 📌 Python Conditional Statements Notes  

#### 🔹 **Conditional Statements Kya Hain?**  
Python me **Conditional Statements** ka use decision making ke liye hota hai. Yeh program ko different conditions ke basis pe alag-alag actions execute karne ki permission dete hain. 

#### 🔹 **if, elif, else Statement**  
```python
age = 22

if age < 13:
    print("Child")
elif age < 20:
    print("Teenager")
elif age < 60:  # Removed `else`
    print("Adult")
else:
    print("Senior")  # Removed parentheses
```
📌 **Explanation:**
- `if` condition check karega agar age 13 se chhoti hai to "Child" print karega.
- `elif` check karega agar age 13 aur 20 ke beech hai to "Teenager" print karega.
- `elif` 60 se chhoti age ke liye "Adult" print karega.
- `else` condition execute hogi agar age 60 ya usse zyada ho.

---

#### 🔹 **Conditional Expression (Ternary Operator)**
```python
age = 22
day = "Wednesday"
price = 12 if age >= 18 else 8  # Short if-else condition

if day == "Wednesday":
    # price = price -2
    price -= 2  # Short-hand for price = price - 2

print(price)
```
📌 **Explanation:**
- `price = 12 if age >= 18 else 8` ek **ternary operator** hai jo short-hand way me if-else ka kaam karta hai.
- Agar `day` Wednesday hai to price me se `2` minus kar diya jayega.

---

#### 🔹 **Multiple Conditions Using elif**
```python
scr = 85

if scr >= 90:
    grade = "A"
elif scr >= 80:  # Fixed 'esif' to 'elif' and '=>' to '>='
    grade = "B"
elif scr >= 70:
    grade = "C"
elif scr >= 60:
    grade = "D"
else:
    grade = "E"

print("Grade:", grade)
```
📌 **Explanation:**
- Score ke basis pe ek grade assign kiya jata hai.
- `if` aur `elif` conditions se different score ranges ke liye alag grades milte hain.
- `else` tab execute hoga jab score 60 se kam hoga.

---

### 🔹 **Extra Conditional Questions**

#### ✅ **Question 4: Even or Odd Number Check**
```python
num = 15

if num % 2 == 0:
    print("Even Number")
else:
    print("Odd Number")
```
📌 **Explanation:**
- Agar `num` ko 2 se divide karne par remainder 0 aata hai to woh **even** hoga.
- Warna woh **odd** number hoga.

---

#### ✅ **Question 5: Leap Year Checker**
```python
year = 2024

if (year % 4 == 0 and year % 100 != 0) or (year % 400 == 0):
    print("Leap Year")
else:
    print("Not a Leap Year")
```
📌 **Explanation:**
- Ek year **leap year** tab hota hai jab:
  1. Woh 4 se divisible ho **aur** 100 se divisible na ho.
  2. Ya phir woh 400 se divisible ho.
- Agar yeh dono conditions fail hoti hain to woh leap year nahi hoga.

---

#### ✅ **Question 6: Positive, Negative or Zero Check**
```python
num = -5

if num > 0:
    print("Positive Number")
elif num < 0:
    print("Negative Number")
else:
    print("Zero")
```
📌 **Explanation:**
- Agar `num` zero se bada hai to "Positive Number" print hoga.
- Agar `num` zero se chhota hai to "Negative Number" print hoga.
- Agar `num` zero hai to "Zero" print hoga.

---

#### ✅ **Question 7: Largest Among Three Numbers**
```python
a, b, c = 5, 12, 8

if a >= b and a >= c:
    print("Largest Number:", a)
elif b >= a and b >= c:
    print("Largest Number:", b)
else:
    print("Largest Number:", c)
```
📌 **Explanation:**
- Yeh program teen numbers me se sabse bada number find karega.
- `if` condition check karegi agar `a` bada ya barabar hai `b` aur `c` se to `a` largest hoga.
- `elif` check karega agar `b` bada ya barabar hai `a` aur `c` se to `b` largest hoga.
- `else` condition execute hogi agar `c` sabse bada hoga.

---

### ✅ **Key Points:**
1. **if, elif, else** ka use decision making ke liye hota hai.
2. **Ternary operator (`condition ? true_value : false_value`)** ka short-hand syntax use kar sakte hain.
3. **Multiple conditions (`elif`)** ka use karke different cases handle kar sakte hain.
4. **Even-Odd check**, **Leap Year check**, **Positive-Negative check**, aur **Largest among three numbers** jaise conditions common scenarios me useful hote hain.

---

