# 🐍 Python 全方位實作題庫 Vol.2 (Weeks 5-8)
# Python Comprehensive Lab Manual (W05-W08)

本文件為課程題庫的第二部分，涵蓋資料結構、函式與模組化設計。

---

## 📦 Week 05: 列表與元組 (Lists & Tuples)
**主題**: List 操作 (CRUD), Slicing, Methods, Tuples, 2D Lists

### 🏗️ 課堂練習 (Practice Labs 1-20)
1.  **P05-01 Create**: 建立包含 5 個水果的 List。
2.  **P05-02 Access**: 印出第一個和最後一個元素。
3.  **P05-03 Update**: 修改 index 2 的值。
4.  **P05-04 Append**: 在末尾新增元素。
5.  **P05-05 Insert**: 在 index 1 插入元素。
6.  **P05-06 Remove**: 移除指定值的元素。
7.  **P05-07 Pop**: 移除並回傳最後一個元素。
8.  **P05-08 Len**: 計算 List 長度。
9.  **P05-09 Sort**: 數字列表排序 (小到大).
10. **P05-10 Reverse**: 反轉列表。
11. **P05-11 Slice Basic**: 取前三個 `[:3]`.
12. **P05-12 Slice Middle**: 取中間 `[1:4]`.
13. **P05-13 Loop List**: `for item in list`.
14. **P05-14 Check In**: `if "Apple" in fruits`.
15. **P05-15 Index**: 找出 "Apple" 的索引值。
16. **P05-16 Count**: 計算某元素出現次數。
17. **P05-17 Tuple Init**: 建立座標 Tuple `(10, 20)`.
18. **P05-18 Tuple Unpack**: `x, y = pos`.
19. **P05-19 List to Tuple**: `tuple(my_list)`.
20. **P05-20 Clear**: 清空列表。

### 🧠 隨堂測驗 (Quiz Labs 1-10)
1.  **Q05-01**: 成績統計 - 輸入 5 個成績，算出平均、最高、最低。
2.  **Q05-02**: 排除不及格 - 將低於 60 分的移除。
3.  **Q05-03**: 矩陣加法 - 兩個長度相同的 List 相加 (Elem-wise).
4.  **Q05-04**: 尋找重複 - 找出 List 中重複出現的元素。
5.  **Q05-05**: 凱薩密碼 - 利用 List 將字串位移加密 (A->B, B->C).
6.  **Q05-06**: 蛇身模擬 - 建立座標 List, 模擬 "移動" (Insert Head, Pop Tail).
7.  **Q05-07**: 合併列表 - 使用 `+` 和 `extend()` 的差異實作。
8.  **Q05-08**: 切片反轉 - 使用 `[::-1]` 檢查迴文 (Palindrome).
9.  **Q05-09**: 二維列表 - 印出 3x3 矩陣的對角線元素。
10. **Q05-10**: 抽籤程式 - 使用 `random.choice` 從 List 隨機選人。

---

## 📚 Week 06: 字典與集合 (Dicts & Sets)
**主題**: Key-Value Pairs, JSON 概念, Set 唯一性

### 🏗️ 課堂練習 (Practice Labs 1-20)
1.  **P06-01 Create Dict**: 建立學生資料 `{name: "Amy", age: 20}`.
2.  **P06-02 Access**: 透過 Key 取得 Value.
3.  **P06-03 Add/Update**: 新增 `score` 或修改 `age`.
4.  **P06-04 Del**: 刪除某個 Key.
5.  **P06-05 Keys**: 印出所有 Keys (`.keys()`).
6.  **P06-06 Values**: 印出所有 Values (`.values()`).
7.  **P06-07 Items**: 印出 Pair (`.items()`).
8.  **P06-08 Get**: 使用 `.get()` 避免 Error。
9.  **P06-09 Check Key**: `if "name" in student`.
10. **P06-10 Nested**: 字典內包含 List `{scores: [90, 80]}`.
11. **P06-11 Create Set**: `{1, 2, 3}`.
12. **P06-12 Add Set**: `.add()`.
13. **P06-13 Remove Set**: `.remove()`.
14. **P06-14 Set Unique**: 將 List 轉 Set 去除重複。
15. **P06-15 Union**: 聯集 `|`.
16. **P06-16 Intersection**: 交集 `&`.
17. **P06-17 Difference**: 差集 `-`.
18. **P06-18 Dict Loop**: `for k, v in d.items()`.
19. **P06-19 List of Dicts**: `[{...}, {...}]`.
20. **P06-20 Clear**: 清空 Dict.

### 🧠 隨堂測驗 (Quiz Labs 1-10)
1.  **Q06-01**: 單字計數器 - 統計文章中每個字出現次數。
2.  **Q06-02**: 通訊錄系統 - 實作查詢、新增手機號碼功能。
3.  **Q06-03**: 摩斯密碼翻譯 - 建立對照表 Dict 進行編碼。
4.  **Q06-04**: 大樂透選號 - 使用 Set 產生 6 個不重複隨機數。
5.  **Q06-05**:購物車加總 - `{"apple": 30, "banana": 20}` 加總 Values.
6.  **Q06-06**: 及格名單 - 從 `{"Amy": 50, "Bob": 80}` 篩選出及格者 Keys.
7.  **Q06-07**: 共同好友 - 兩個 User 的好友 Sets 取交集。
8.  **Q06-08**: 州名縮寫查詢 - 輸入縮寫 output 全名。
9.  **Q06-09**: 巢狀資料解析 - 取得 `data["users"][0]["email"]`.
10. **Q06-10**: JSON 格式模擬 - 將 Dict 轉字串印出。

---

## 🛠️ Week 07: 函式與模組 (Functions)
**主題**: Def, Arguments, Return, Lambda, Modules

### 🏗️ 課堂練習 (Practice Labs 1-20)
1.  **P07-01 Def Basic**: 定義 `say_hello()` 並呼叫。
2.  **P07-02 Param**: 定義 `greet(name)`.
3.  **P07-03 Add**: 定義 `add(a, b)` 並 print。
4.  **P07-04 Return**: 改為 `return a + b`.
5.  **P07-05 Docstring**: 為函式寫說明文件。
6.  **P07-06 Default Arg**: `def power(base, exp=2)`.
7.  **P07-07 Keyword Arg**: `func(a=1, b=2)`.
8.  **P07-08 Scope**: 區域變數 vs 全域變數觀察。
9.  **P07-09 Lambda**: `sq = lambda x: x*x`.
10. **P07-10 List Pass**: 傳入 List 並修改 (Pass by ref).
11. **P07-11 Import Math**: 使用 `math.sqrt`.
12. **P07-12 Import Random**: `random.randint`.
13. **P07-13 From Import**: `from math import pi`.
14. **P07-14 Import As**: `import datetime as dt`.
15. **P07-15 Time Sleep**: `time.sleep(1)`.
16. **P07-16 Dice Roll**: 封裝擲骰子函式。
17. **P07-17 Check Even**: 函式回傳 Bool.
18. **P07-18 Max Function**: 自製 max 函式。
19. **P07-19 Sum Function**: 自製 sum 函式。
20. **P07-20 None Return**: 觀察無 return 的函式回傳值。

### 🧠 隨堂測驗 (Quiz Labs 1-10)
1.  **Q07-01**: 萬用計算機 - 傳入 `(num1, num2, op)` 回傳結果。
2.  **Q07-02**: 質數檢查函式 - `is_prime(n) -> bool`.
3.  **Q07-03**: 溫度轉換模組 - 包含 C2F 和 F2C 兩個函式。
4.  **Q07-04**: 清單過濾器 - 傳入 List 與閥值，回傳篩選後的 List。
5.  **Q07-05**: 遞迴階乘 - `factorial(n)` 使用 Recursion。
6.  **Q07-06**:猜拳邏輯 - 封裝 `check_winner(p1, p2)`.
7.  **Q07-07**: 圓形計算庫 - 包含面積與周長函式。
8.  **Q07-08**: 密碼產生器 - 封裝產生 n 碼隨機字串的邏輯。
9.  **Q07-09**: 統計函式包 - 傳入 List 回傳 `(min, max, avg)` Tuple.
10. **Q07-10**: 裝飾器初探 - 定義一個簡單的 `@logger` (Advanced).

---

## 📝 Week 08: 期中綜合評量 (Midterm Review)
**主題**: 綜合應用 Weeks 1-7 之技能

### 🏗️ 課堂練習 (Practice Labs 1-20)
*本週練習為複習與除錯 (Debug)*
1.  **P08-01 Debug Syntax**: 修正缺少冒號的錯誤。
2.  **P08-02 Debug Indent**: 修正縮排錯誤。
3.  **P08-03 Debug Type**: 修正 `str + int` 錯誤。
4.  **P08-04 Debug Logic**: 修正無窮迴圈。
5.  **P08-05 Review Loop**: 畫出菱形。
6.  **P08-06 Review List**: 實作 Bubble Sort (氣泡排序) 基礎。
7.  **P08-07 Review Dict**: 合併兩個字典。
8.  **P08-08 Review Func**: 函式預設值陷阱 (Empty List).
9.  **P08-09 Algo**: 二分搜尋法 (Binary Search) 概念實作。
10. **P08-10 ASCII Art**: 印出複雜圖形。
11. **P08-11 Data Clean**: 清理 List 中的空字串。
12. **P08-12 Matrix Trans**: 矩陣轉置 (3x2 -> 2x3).
13. **P08-13 String Format**: 對齊輸出 (Ljust, Rjust).
14. **P08-14 Validation**: 檢查 Email 格式 (簡易版).
15. **P08-15 Shopping Cart**: 綜合 Dict 與 Calculation.
... (16-20 為自由複習)

### 🧠 隨堂測驗 (Quiz Labs 1-10)
*期中考題組 (Mini Project)*
1.  **Q08-01**: 成績系統完整版 - 支援新增、查詢、列出不及格、計算平均。
2.  **Q08-02**: 簡易文字冒險遊戲 - 結合 If/Else, Input, Loop, State.
3.  **Q08-03**: 訂票系統 - 選擇座位 (2D List 狀態更新).
4.  **Q08-04**: 資料分析 - 給定一長串數值字串，解析並統計分佈。
5.  **Q08-05**: 密碼強度檢測器 V2 (包含大小寫、數字、長度檢查).
6.  **Q08-06**: 猜數字 AI - 寫一個程式自動猜使用者的數字 (Binary Search).
7.  **Q08-07**: 日期計算 - 計算距離跨年還有幾天。
8.  **Q08-08**: 凱薩密碼解密 - 暴力破解位移值 (Brute force).
9.  **Q08-09**: 購物車結帳 - 包含會員折扣、滿額贈、庫存扣除。
10. **Q08-10**: 井字遊戲邏輯 - 判斷 3x3 版面是否有連線。
