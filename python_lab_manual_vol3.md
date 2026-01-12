# 🐍 Python 全方位實作題庫 Vol.3 (Weeks 9-12)
# Python Comprehensive Lab Manual (W09-W12)

本文件涵蓋進階主題：檔案處理、物件導向 (OOP) 與 Pygame 專案啟動。

---

## 📂 Week 09: 檔案與例外處理 (Files & Exceptions)
**主題**: File I/O, CSV, Try/Except, Defensive Coding

### 🏗️ 課堂練習 (Practice Labs 1-20)
1.  **P09-01 Write**: 寫入文字檔 `open('test.txt', 'w')`.
2.  **P09-02 Read**: 讀取文字檔 `.read()`.
3.  **P09-03 ReadLine**: 逐行讀取 `.readline()`.
4.  **P09-04 ReadLines**: 讀入列表 `.readlines()`.
5.  **P09-05 Append**: 附加模式 `'a'`.
6.  **P09-06 With**: 使用 `with open...` 自動關閉。
7.  **P09-07 Loop File**: `for line in f`.
8.  **P09-08 Strip**: 去除換行符號 `.strip()`.
9.  **P09-09 Encoding**: UTF-8 編碼設定 `encoding='utf-8'`.
10. **P09-10 CSV Split**: 使用 `.split(',')` 解析 CSV 行。
11. **P09-11 Try-Except**: 捕捉 `ZeroDivisionError`.
12. **P09-12 Catch FileErr**: 捕捉 `FileNotFoundError`.
13. **P09-13 Catch ValueErr**: 捕捉 `ValueError` (輸入文字轉數字).
14. **P09-14 Multiple Except**: 捕捉多種錯誤。
15. **P09-15 Else**: 無錯誤時執行。
16. **P09-16 Finally**: 無論如何都執行 (Close helper).
17. **P09-17 Raise**: 主動拋出錯誤 `raise ValueError`.
18. **P09-18 Exist Check**: 使用 `os.path.exists`.
19. **P09-19 Delete File**: 使用 `os.remove`.
20. **P09-20 Rename**: 使用 `os.rename`.

### 🧠 隨堂測驗 (Quiz Labs 1-10)
1.  **Q09-01**: 日誌系統 - 寫入 `[Time] Event` 到 log.txt.
2.  **Q09-02**: 文檔複製 - 將 A.txt 內容複製到 B.txt.
3.  **Q09-03**: 簡單記帳 - 讀取 CSV (Item,Price), 計算總合。
4.  **Q09-04**: 安全除法器 - 持續輸入直到成功除法 (Loop + Try).
5.  **Q09-05**: 設定檔讀取 - 讀取 `config.txt` (格式 `key=value`) 轉為 Dict.
6.  **Q09-06**: 成績單生成 - 將 Student Dict 寫入為 CSV 格式。
7.  **Q09-07**: 替換文字 - 讀取檔案，將所有 "Happy" 改為 "Joy"，存檔。
8.  **Q09-08**: 最高分持久化 - 比較當前分數與檔案中最高分。
9.  **Q09-09**: 資料庫模擬 - 實作簡易的 `insert_record(file, record)` 函式。
10. **Q09-10**: 異常日誌 - 捕捉程式錯誤並將錯誤訊息寫入 `error.log`.

---

## 🏗️ Week 10: 物件導向基礎 (OOP)
**主題**: Class, Object, Attribute `self.var`, Method `self.func()`

### 🏗️ 課堂練習 (Practice Labs 1-20)
1.  **P10-01 Class Def**: 定義空類別 `class Car: pass`.
2.  **P10-02 Object**: 實例化 `c = Car()`.
3.  **P10-03 Init**: 定義 `__init__`.
4.  **P10-04 Attribute**: `self.color = color`.
5.  **P10-05 Method**: 定義 `drive(self)`.
6.  **P10-06 Self**: 理解 self 的意義 (Print id).
7.  **P10-07 Multiple Objs**: 建立多個實例，觀察屬性獨立性。
8.  **P10-08 Default Attr**: Init 中設定預設值。
9.  **P10-09 Modifying Attr**: 直接修改 `c.color = "Red"`.
10. **P10-10 Method Call**: `c.drive()`.
11. **P10-11 Str Method**: 定義 `__str__` 以美化 print.
12. **P10-12 Param Method**: `drive(km)` 扣油量。
13. **P10-13 State Check**: `is_empty()` 回傳 Bool.
14. **P10-14 Class Var**: 類別變數 (所有實例共享).
15. **P10-15 Private Var**: `self.__secret` 封裝。
16. **P10-16 Getter/Setter**: 透過方法存取私有變數。
17. **P10-17 Inheritance**: `class EV(Car):`.
18. **P10-18 Override**: 子類別覆寫父類別方法。
19. **P10-19 Super**: `super().__init__()`.
20. **P10-20 Composition**: 類別中包含其他類別 (Car has a Engine).

### 🧠 隨堂測驗 (Quiz Labs 1-10)
1.  **Q10-01**: 學生類別 - 包含 `study()` 增加知識值，`sleep()` 恢復體力。
2.  **Q10-02**:銀行帳戶 - 實作存款、提款、轉帳 (Transfer).
3.  **Q10-03**: 矩形類別 - 屬性長寬，方法 `area()`, `perimeter()`.
4.  **Q10-04**: 書籍管理 - Book 類別，Library 類別 (List of Books).
5.  **Q10-05**: 購物車 OOP - Item 類別，Cart 類別 (計算總價).
6.  **Q10-06**: RPG 角色 - Warrior 繼承 Character, 覆寫 `attack()`.
7.  **Q10-07**: 貪食蛇原型 - `Snake` 類別，屬性 `body` (List), `direction`.
8.  **Q10-08**: 座標點類別 - `Point(x, y)`, 實作 `distance_to(p2)`.
9.  **Q10-09**: 堆疊實作 - 使用 Class 包裝 List 實作 Stack (Push/Pop).
10. **Q10-10**: 寵物遊戲 - 實作 Tamagotchi 邏輯 (Hunger, Happiness).

---

## 🎮 Week 11: Pygame 專案啟動 (Project Setup)
**主題**: VS Code Setup, Pygame Window, Event Loop, Drawing

### 🏗️ 課堂練習 (Practice Labs 1-20)
1.  **P11-01 Install**: `pip install pygame`.
2.  **P11-02 Import**: `import pygame` check ver.
3.  **P11-03 Init**: `pygame.init()`.
4.  **P11-04 Window**: `set_mode((800, 600))`.
5.  **P11-05 Title**: `set_caption("Snake")`.
6.  **P11-06 Game Loop**: `while running:`.
7.  **P11-07 Event Get**: `pygame.event.get()`.
8.  **P11-08 Quit**: Handle `pygame.QUIT`.
9.  **P11-09 Colors**: 定義 RGB Tuple `(255, 0, 0)`.
10. **P11-10 Fill**: `screen.fill(COLOR)`.
11. **P11-11 Flip**: `display.flip()` Update screen.
12. **P11-12 Draw Rect**: `draw.rect()`.
13. **P11-13 Rect Obj**: 建立 `pygame.Rect` 物件。
14. **P11-14 Draw Circle**: `draw.circle()`.
15. **P11-15 Draw Line**: `draw.line()`.
16. **P11-16 Clock**: `time.Clock()`.
17. **P11-17 FPS**: `clock.tick(60)`.
18. **P11-18 Key Press**: `if event.key == K_UP`.
19. **P11-19 Mouse**: Get mouse position.
20. **P11-20 Cleanup**: `pygame.quit()`, `sys.exit()`.

### 🧠 隨堂測驗 (Quiz Labs 1-10)
*Pygame 初體驗*
1.  **Q11-01**: 紅變藍 - 點擊滑鼠切換背景顏色。
2.  **Q11-02**: 移動方塊 - 使用方向鍵控制方塊座標 (continuous).
3.  **Q11-03**: 跳動球 - 球碰到視窗邊緣反彈 (Bouncing Ball).
4.  **Q11-04**: 跟隨滑鼠 - 圓圈跟隨滑鼠移動。
5.  **Q11-05**: 網格繪製 - 使用迴圈畫出棋盤格線 (Grid).
6.  **Q11-06**: 隨機顏色 - 按空白鍵隨機改變方塊顏色。
7.  **Q11-07**: 圖片載入 - 載入並顯示一張圖片 (Surface).
8.  **Q11-08**: 文字顯示 - 使用 Font 顯示 "Hello Pygame".
9.  **Q11-09**: 畫布清除 - 每一幀重畫背景的重要性體驗 (殘影實驗).
10. **Q11-10**: 簡易塗鴉板 - 滑鼠按住時繪製線條。

---

## 🐍 Week 12: 類別設計 (Class Design for Snake)
**主題**: Snake Class, Food Class, Grid System logic

### 🏗️ 課堂練習 (Practice Labs 1-20)
1.  **P12-01 Grid Constants**: 定義 `GRID_SIZE`, `WIDTH`, `HEIGHT`.
2.  **P12-02 Snake Init**: `self.body = [(10,10), (9,10)]`.
3.  **P12-03 Draw Snake**: 遍歷 body 繪製 Rect.
4.  **P12-04 Direction Enum**: 使用 Enum 定義 UP, DOWN...
5.  **P12-05 Valid Move Test**: 測試座標 (x, y) 是否在視窗內。
6.  **P12-06 Food Init**: `self.pos = (x, y)`.
7.  **P12-07 Random Spawn**: 產生隨機網格座標 Logic.
8.  **P12-08 Draw Food**: 繪製紅色圓形食物。
9.  **P12-09 Game Class**: 建立 Game 管理類別。
10. **P12-10 Integration**: 在 Game 中實例化 Snake 與 Food.
11. **P12-11 Snake Head**: `body[0]` 存取練習。
12. **P12-12 Vector Math**: `(x+dx, y+dy)` 練習。
13. **P12-13 Delta Dict**: `{UP: (0, -1), ...}` mapping.
14. **P12-14 Opposite Dir**: 判斷是否為反方向 Tuple.
15. **P12-15 Color Constants**: 定義 SNAKE_GREEN, FOOD_RED.
16. **P12-16 Rect Inflate**: 縮小 Rect 做出間隔效果。
17. **P12-17 Border Radius**: 繪製圓角矩形。
18. **P12-18 Static Method**: 理解 helper method.
19. **P12-19 Type Hinting**: `def move(self) -> None:`.
20. **P12-20 Unit Test**: 測試 Snake 初始化長度。

### 🧠 隨堂測驗 (Quiz Labs 1-10)
1.  **Q12-01**: 蛇頭識別 - 繪製時將蛇頭改為深綠色，蛇身淺綠。
2.  **Q12-02**: 食物重疊檢查 - 確保 spawn 不會生在 snake body 上。
3.  **Q12-03**: 網格對齊 - 確保 rect 座標是 `col * GRID_SIZE`.
4.  **Q12-04**: 方向鎖定 - 實作 `change_direction` 避免 180 度迴轉。
5.  **Q12-05**: 眼睛繪製 - 在蛇頭 rect 上畫兩個小圓點 (方向正確性不拘).
6.  **Q12-06**: 閃爍食物 - 讓食物顏色隨時間變化 (sin wave or random).
7.  **Q12-07**: 多重食物 - 支援畫面上同時有多個食物。
8.  **Q12-08**: 穿牆邏輯 (實驗) - `x = x % GRID_WIDTH`.
9.  **Q12-09**: 重置機制 - 實作 `reset()` 將蛇回到中心。
10. **Q12-10**: 靜態畫面整合 - 顯示蛇、食物、網格的靜態構圖。
