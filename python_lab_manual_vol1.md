# 🐍 Python 全方位實作題庫 Vol.1 (Weeks 1-4)
# Python Comprehensive Lab Manual (W01-W04)

本題庫為 16 週 PBL 課程設計，每週包含 **20 題課堂練習 (Practice)** 與 **10 題隨堂測驗 (Quiz)**，共計 480 題。此文件包含前 4 週共 120 題。

---

## 📅 Week 01: Python 啟航 (Start)
**主題**: 變數、資料型態 (str, int, float)、基本輸入輸出
**Core**: `print()`, `input()`, `f-string`

### 🏗️ 課堂練習 (Practice Labs 1-20)
1.  **P01-01 Hello**: 印出 "Hello, Python!"。
    ```python
    print("Hello, Python!")
    ```
2.  **P01-02 My Name**: 宣告變數 `name` 並印出。
    ```python
    name = "Alice"
    print(name)
    ```
3.  **P01-03 Self Intro**: 結合字串印出 "I am [Name]".
    ```python
    print("I am " + name)
    ```
4.  **P01-04 Basic Math**: 計算 10 + 5 並印出。
    ```python
    print(10 + 5)
    ```
5.  **P01-05 Multi-print**: 同一行印出多個值 `print(1, 2, 3)`.
    ```python
    print(1, 2, 3)
    ```
6.  **P01-06 Separator**: 使用 `sep` 參數 `print(1, 2, sep="-")`.
    ```python
    print("2023", "01", "01", sep="-")
    ```
7.  **P01-07 End param**: 使用 `end` 參數不換行。
    ```python
    print("Hello", end=" ")
    print("World")
    ```
8.  **P01-08 Variables**: 交換兩個變數的值 (Temp var)。
    ```python
    a, b = 1, 2
    temp = a; a = b; b = temp
    print(a, b)
    ```
9.  **P01-09 Python Swap**: Python 風格交換變數 `a, b = b, a`.
    ```python
    a, b = 10, 20
    a, b = b, a
    print(a, b)
    ```
10. **P01-10 Input**: 取得使用者名字並打招呼。
    ```python
    name = input("Name? ")
    print(f"Hi, {name}")
    ```
11. **P01-11 Input Int**: 輸入年齡並轉為整數。
    ```python
    age = int(input("Age? "))
    print(age)
    ```
12. **P01-12 Input Float**: 輸入身高並轉為浮點數。
    ```python
    h = float(input("Height? "))
    print(h)
    ```
13. **P01-13 Calc Age**: 輸入出生年，計算今年幾歲 (以 2026 為例)。
    ```python
    year = int(input("Year? "))
    print(2026 - year)
    ```
14. **P01-14 F-String**: 使用 f-string 格式化輸出。
    ```python
    score = 95
    print(f"Score: {score}")
    ```
15. **P01-15 Float Format**: f-string 控制小數點 `.2f`.
    ```python
    pi = 3.14159
    print(f"{pi:.2f}")
    ```
16. **P01-16 Type Check**: 使用 `type()` 檢查變數型態。
    ```python
    print(type(10))
    print(type(3.14))
    ```
17. **P01-17 String Repeat**: 字串乘法 `print("A" * 5)`.
    ```python
    print("Go" * 3)
    ```
18. **P01-18 String Concat**: 字串加法。
    ```python
    s = "Py" + "thon"
    print(s)
    ```
19. **P01-19 Area Calc**: 輸入長寬計算面積。
    ```python
    w = int(input("W? "))
    h = int(input("H? "))
    print(w * h)
    ```
20. **P01-20 Divider**: 印出分隔線 `print("-" * 20)`.
    ```python
    print("=" * 20)
    ```

### 🧠 隨堂測驗 (Quiz Labs 1-10)
1.  **Q01-01**: 修正語法錯誤 `Print("Hi")` to `print("Hi")`.
2.  **Q01-02**: 變數命名規則，判斷 `2nd_place` 合法性 (非法)。
3.  **Q01-03**: 輸入兩個數字，印出總和 (需轉型)。
    ```python
    a = int(input())
    b = int(input())
    print(a + b)
    ```
4.  **Q01-04**: 製作名片框 (使用 `*`).
    ```python
    name = input("Name: ")
    print("*" * 10)
    print(f"* {name} *")
    print("*" * 10)
    ```
5.  **Q01-05**: 單位換算，公尺轉公分。
6.  **Q01-06**: 秒數轉分鐘 (初步概念，不求餘數)。 `sec / 60`.
7.  **Q01-07**: 計算圓面積 (固定 pi=3.14).
8.  **Q01-08**: 顯示引號 (Escape char) `print("I\'m OK")`.
9.  **Q01-09**: 多行字串 (Triple quotes).
    ```python
    print("""Line 1
    Line 2""")
    ```
10. **Q01-10**: 綜合題 - 自我介紹產生器 V2 (包含 Name, Age, Hobby).

---

## ➕ Week 02: 運算與邏輯 (Operators)
**主題**: 算術運算、比較運算、邏輯運算 (and, or, not)、IPO 模型

### 🏗️ 課堂練習 (Practice Labs 1-20)
1.  **P02-01 Add**: `a + b`
2.  **P02-02 Sub**: `a - b`
3.  **P02-03 Mul**: `a * b`
4.  **P02-04 Div**: `a / b` (Float result)
5.  **P02-05 Floor Div**: `a // b` (整除)
    ```python
    print(10 // 3) # 3
    ```
6.  **P02-06 Modulo**: `a % b` (取餘數).
    ```python
    print(10 % 3) # 1
    ```
7.  **P02-07 Power**: `a ** b` (次方).
    ```python
    print(2 ** 3) # 8
    ```
8.  **P02-08 PEMDAS**: `(2 + 3) * 5` 優先順序。
9.  **P02-09 Assignment**: `x += 1`.
10. **P02-10 More Assign**: `x *= 2`.
11. **P02-11 Equal**: `==` 判斷相等。
12. **P02-12 Not Equal**: `!=` 判斷不等。
13. **P02-13 Greater**: `>` 判斷大於。
14. **P02-14 Logic AND**: `True and False`.
15. **P02-15 Logic OR**: `True or False`.
16. **P02-16 Logic NOT**: `not True`.
17. **P02-17 In Range**: `10 < x < 20`.
18. **P02-18 BMI Step 1**: 計算 `h_meter = h_cm / 100`.
19. **P02-19 BMI Step 2**: 計算 `w / (h ** 2)`.
20. **P02-20 Boolean Int**: `bool(1)` vs `bool(0)`.

### 🧠 隨堂測驗 (Quiz Labs 1-10)
1.  **Q02-01**: 餘數應用 - 判斷奇偶數 (印出 0 或 1)。 `n % 2`.
2.  **Q02-02**: 華氏轉攝氏公式實作。 `(F-32) * 5/9`.
3.  **Q02-03**: 簡單匯率計算機 (TWD -> USD).
4.  **Q02-04**: 時間換算 - 總秒數轉 "時:分:秒" (利用 // 和 %).
    ```python
    s = int(input())
    m = s // 60
    rem_s = s % 60
    print(f"{m}m {rem_s}s")
    ```
5.  **Q02-05**: 優惠計算 - 打八折 `price * 0.8`.
6.  **Q02-06**: 三角形面積 `(b * h) / 2`.
7.  **Q02-07**: 複合比較 `age >= 18 and code == "PASS"`.
8.  **Q02-08**: 互斥條件 `is_weekend or is_holiday`.
9.  **Q02-09**: 邏輯短路測試 (Short-circuit).
10. **Q02-10**: 收銀台 - 計算總價與找零，並判斷錢是否足夠 (Bool).

---

## ❓ Week 03: 決策流程 (Conditionals)
**主題**: If, Elif, Else, 巢狀判斷

### 🏗️ 課堂練習 (Practice Labs 1-20)
1.  **P03-01 Simple If**: 若 `x > 0` 印出 Positive.
2.  **P03-02 If-Else**: 正數或非正數。
3.  **P03-03 Odd/Even**: 使用 `if n % 2 == 0`.
4.  **P03-04 Pass Check**: 分數 >= 60 及格，否則當掉。
5.  **P03-05 Password**: 檢查輸入字串是否等於 "secret".
6.  **P03-06 Elif**: 正數、負數、零。
7.  **P03-07 Grades**: A(90), B(80), C(60), F.
8.  **P03-08 Nested If**: 先檢查是否成年，再檢查是否有駕照。
9.  **P03-09 Age Group**: Child, Teen, Adult, Elder.
10. **P03-10 Multiple Cond**: `if a > 0 and b > 0`.
11. **P03-11 String Compare**: `name == "Alice"`.
12. **P03-12 Length Check**: `len(pwd) >= 8`.
13. **P03-13 Not Empty**: `if name:` (空字串為 False).
14. **P03-14 Login Mock**: 帳號 AND 密碼皆正確。
15. **P03-15 Discount**: 滿千送百邏輯。
16. **P03-16 Max of 2**: 印出 a, b 較大者。
17. **P03-17 Ternary Op**: `msg = "Yes" if ok else "No"`.
18. **P03-18 Membership**: `if "a" in "apple"`.
19. **P03-19 Not In**: `if "x" not in "apple"`.
20. **P03-20 Bool Check**: `if is_raining:`.

### 🧠 隨堂測驗 (Quiz Labs 1-10)
1.  **Q03-01**: 閏年判斷 (經典面試題).
    ```python
    y = int(input())
    if (y%4==0 and y%100!=0) or (y%400==0): print("Leap")
    ```
2.  **Q03-02**: 三數取最大值 (不使用 max 函式).
3.  **Q03-03**: 簡易計算機 (輸入兩數與運算符號 +, -, *, /).
4.  **Q03-04**: 餐廳點餐 - 判斷餘額是否足夠買 A 餐或 B 餐.
5.  **Q03-05**: BMI 判讀 - 過輕、正常、過重、肥胖.
6.  **Q03-06**: 性向測驗 - 簡單的 Yes/No 分支問答.
7.  **Q03-07**: 座標象限判斷 (輸入 x, y 判斷 I, II, III, IV).
8.  **Q03-08**: 停車費計算 (未滿半小時免費，超過每小時 40).
9.  **Q03-09**: 三角形判斷 (兩邊和大於第三邊).
10. **Q03-10**: 剪刀石頭布 (單局勝負判斷).

---

## 🔄 Week 04: 迴圈 (Loops)
**主題**: While, For, Range, Break, Continue, 巢狀迴圈

### 🏗️ 課堂練習 (Practice Labs 1-20)
1.  **P04-01 While 5**: 印出 1 到 5.
2.  **P04-02 While Sum**: 計算 1 到 10 的和。
3.  **P04-03 Countdown**: 倒數 10 到 1.
4.  **P04-04 For Range**: `for i in range(5)`.
5.  **P04-05 For Range 2**: `range(1, 6)`.
6.  **P04-06 For Step**: `range(0, 10, 2)` (偶數).
7.  **P04-07 String Loop**: 逐字印出字串 `for char in "Python"`.
8.  **P04-08 Sum 100**: 使用 for 計算 1-100 總和。
9.  **P04-09 Factorial**: 計算 n! (階乘).
10. **P04-10 Step Back**: `range(10, 0, -1)`.
11. **P04-11 Break**: 遇到 5 就停止迴圈。
12. **P04-12 Continue**: 跳過 3 的倍數。
13. **P04-13 Input Loop**: 持續輸入直到 user 輸入 "q".
14. **P04-14 Nested Loop**: 印出 3x3 矩陣座標 `(0,0), (0,1)...`.
15. **P04-15 Star Line**: 印出 n 個星星 `print("*", end="")`.
16. **P04-16 Square**: 印出 NxN 的星星方塊。
17. **P04-17 Triangle**: 印出直角三角形。
18. **P04-18 Else in For**: 迴圈正常結束後執行。
19. **P04-19 Enumerate**: `idx, val` 用法初步。
20. **P04-20 Accumulator**: 累加輸入的數字直到輸入 0.

### 🧠 隨堂測驗 (Quiz Labs 1-10)
1.  **Q04-01**: 終極密碼 (Guess Number) - 猜錯提示大小，直到猜對。
2.  **Q04-02**: 九九乘法表 (Nested Loop with formatting).
3.  **Q04-03**: 質數判斷 (Prime Checker) - 檢查是否只能被 1 和自己整除。
4.  **Q04-04**: 金字塔圖形 (置中排列的星星).
5.  **Q04-05**: 費氏數列 (Fibonacci) 前 10 項.
6.  **Q04-06**: 反轉字串 - 不使用 slicing，用迴圈。
7.  **Q04-07**: 尋找最大值 - 輸入 5 個數，找出最大者 (不依賴 list).
8.  **Q04-08**: 存錢計畫 - 每天存 10 元，幾天能存到目標金額？
9.  **Q04-09**: 公因數列舉 - 列出某數的所有因數。
10. **Q04-10**: 數字反轉 - 輸入 123 輸出 321 (Math mathod).
