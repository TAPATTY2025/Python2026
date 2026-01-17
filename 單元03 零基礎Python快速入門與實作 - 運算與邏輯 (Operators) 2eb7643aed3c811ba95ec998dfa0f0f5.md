# 單元03. 零基礎Python快速入門與實作 - 運算與邏輯 (Operators)

## 1. 核心觀念 (Core Concepts)

![image.png](image.png)

---

## 2. 課堂實作 (Practice Labs)

[單元03. 零基礎Python快速入門與實作](https://gamma.app/docs/03-Python-cvzwgbzeupm5p24?mode=doc)

### P02-01 to P02-04 Basic Calc

> 題目: 基本四則運算 (Add, Sub, Mul, Div)。
> 
- **Analysis**: 基本四則運算。

```python
a, b = 10, 3
print(a + b)
print(a - b)
print(a * b)
print(a / b) # 3.333...

```

### P02-05 Floor Div

> 題目: a // b (整除)。
> 
- **Analysis**: 地板除法，無條件捨去小數。

```python
print(10 // 3) # 3

```

### P02-06 Modulo

> 題目: a % b (取餘數)。
> 
- **Analysis**: 取餘數，常用於判斷倍數或是循環 (如時鐘)。

```python
print(10 % 3) # 1

```

### P02-07 Power

> 題目: a ** b (次方)。
> 
- **Analysis**: 次方運算。

```python
print(2 ** 3) # 8

```

### P02-08 PEMDAS

> 題目: (2 + 3) * 5 優先順序。
> 
- **Analysis**: 先乘除後加減，括號優先。

```python
print((2 + 3) * 5) # 25

```

### P02-09 Assignment

> 題目: x += 1。
> 
- **Analysis**: 複合運算子，簡潔程式碼。

```python
x = 5
x += 1 # x = x + 1
print(x)

```

### P02-10 More Assign

> 題目: x *= 2。
> 
- **Analysis**: 複合運算子。

```python
x = 5
x *= 2 # x = x * 2
print(x)

```

### P02-11 to P02-13 Comparison

> 題目: 比較 (Equal, Not Equal, Greater)。
> 
- **Analysis**: 比較結果必定為布林值。

```python
print(5 == 5) # True
print(5 != 3) # True
print(5 > 10) # False

```

### P02-14 to P02-16 Logic

> 題目: 邏輯 (AND, OR, NOT)。
> 
- **Analysis**: 邏輯閘概念。

```python
print(True and False) # False
print(True or False)  # True
print(not True)       # False

```

### P02-17 Range Check

> 題目: 10 < x < 20。
> 
- **Analysis**: Python 允許連寫比較運算子。

```python
x = 15
print(10 < x < 20) # True

```

### P02-18/19 BMI Steps

> 題目: 分步計算 BMI (M to CM, then formula).
> 
- **Analysis**: 分步計算 BMI，運用平方與除法。

```python
h_cm = 180
w_kg = 75
h_m = h_cm / 100
bmi = w_kg / (h_m ** 2)
print(bmi)

```

### P02-20 Boolean Int

> 題目: bool(1) vs bool(0).
> 
- **Analysis**: 非零即為真。

```python
print(bool(1)) # True
print(bool(0)) # False

```

---

## 3. 隨堂測驗 (Quiz Labs)

### Q02-01 Odd/Even

> 題目: 餘數應用 - 判斷奇偶數 (印出 0 或 1)。 n % 2.
> 
- **Analysis**: 利用餘數判斷奇偶 (除以 2 餘 0 為偶，餘 1 為奇)。

```python
Your Show Time

```

### Q02-02 F to C

> 題目: 華氏轉攝氏公式實作。 (F-32) * 5/9.
> 
- **Analysis**: 運算優先序的應用。

```python
Your Show Time

```

### Q02-03 Exchange

> 題目: 簡易匯率計算機 (TWD -> USD).
> 
- **Analysis**: 商業應用基礎。

```python
Your Show Time

```

### Q02-04 Time Logic

> 題目: 時間換算 - 總秒數轉 "時:分:秒"。
> 
- **Analysis**: 結合整除與餘數運算。

```python
Your Show Time

```

### Q02-05 Discount

> 題目: 優惠計算 - 打八折 price * 0.8.
> 
- **Analysis**: 浮點數乘法。

```python
Your Show Time

```

### Q02-06 Triangle

> 題目: 三角形面積 (b * h) / 2.
> 
- **Analysis**: 幾何公式。

```python
Your Show Time

```

### Q02-07 Complex Compare

> 題目: 複合比較 age >= 18 and code == "PASS".
> 
- **Analysis**: 多重條件驗證。

```python
Your Show Time

```

### Q02-08 Mutual Exclusive

> 題目: 互斥條件 is_weekend or is_holiday.
> 
- **Analysis**: 只要滿足其一即可。

```python
Your Show Time

```

### Q02-09 Short-circuit

> 題目: 邏輯短路測試 (Short-circuit).
> 
- **Analysis**: 效率與安全性 (避免除以零)。

```python
Your Show Time

```

### Q02-10 Cashier Bool

> 題目: 收銀台 - 判斷錢是否足夠 (Bool).
> 
- **Analysis**: 用比較運算子直接產生布林值作為結果。

```python
Your Show Time
```

![Untitled](Untitled.png)

# 🎯 Don’t forget update your work into Repository! Cheer up!🎓🚀

## **Reference: Quick Approach to Learn Python**

[Python for Beginners - Learn Python in 1 Hour](https://www.youtube.com/watch?v=kqtD5dpn9C8)

[Python Online Compiler & Interpreter](https://replit.com/languages/python3)

[👩‍💻 Python for Beginners Tutorial](https://www.youtube.com/watch?v=b093aqAZiPU)

[【python】4小時初學者Python教學 #python #python教學 #python入門](https://www.youtube.com/watch?v=zdMUJJKFdsU)

[Python: 5周从入门到精通，听说高考都要考Python啦 |数据应用学院 公开课 (零基础)](https://www.youtube.com/watch?v=WgfZ80Cv4aY)

X

[十分钟学会Python!? 张土汪带你玩编程 (2019)](https://www.youtube.com/watch?v=DRQYOdO9BAU&t=864s)