# Sensor Tower《State of AI Report 2026》解讀報告（草稿）

**來源：** Sensor Tower State of AI Report 2026（PDF，74 頁，使用者上傳）
**性質：** 與每週 AI 新知週報不同 —— 這份不是「新功能/新模型發布」新聞，而是 Sensor Tower 用 App Store / 廣告 / 網站數據做的**實證市場行為報告**，量化了「AI 助理使用者實際在做什麼」。

---

## 為什麼這份報告值得跟過去週報內容對照

過去 W20~W25 週報追蹤的都是「廠商發布了什麼」（Opus 4.8、Dynamic Workflows、Fable 5 下架、Managed Agents Cron 等）。
這份報告補上了我們從沒量化過的一塊：**這些發布實際造成多少用戶行為改變**。以下是幾個我認為「之前完全不知道」、值得跟 Codex 進一步討論/驗證的數字。

---

## 之前不知道的關鍵發現（待討論清單）

### 1. ChatGPT 真實受眾市佔率跌破 50%，且有具體觸發事件
- 2026-03 首次跌破 50%，5 月剩 **46%**（Gemini 28%、Claude 10%）
- 觸發點：2/26 Anthropic 拒絕與美國國防部合作 → 2/28 OpenAI 與美國戰爭部簽約 → ChatGPT 解除安裝量單週 **+202%**
- 3/1~3/5 期間 Claude 單日下載量首次超越 ChatGPT
- **討論點：** 我們之前完全沒追蹤過「企業政治立場 → 用戶解除安裝」這種因果鏈的具體幅度數據，這對任何 AI 公司的公關/政策決策都是一個可量化的風險係數。

### 2. Claude 的商業化轉型幅度比想像中大
- ARPU：2025-09 不到 $0.5 → 2026-05 的 **$2.76**（5倍以上成長，8個月內）
- Claude 在美國的市佔率：5%（2025-12）→ 14%（2026-05）
- **討論點：** 這個 ARPU 成長曲線是否能解釋 Anthropic 為何敢在同期推出 Agent SDK 計費分池（W24週報追蹤的 June 15 billing change）？兩者時間點吻合，可能是同一個「轉向營收最大化」策略的兩個面向。

### 3. Agentic Shopping 已有實證 ROI 數字，不只是概念
- Amazon Rufus：轉換率 >40%（非用戶 ~20%），轉換前停留 40 分鐘（非用戶 15 分鐘）
- Walmart Sparky：用戶 AOV 高 35%，DAU 半年成長近 50%
- Amazon 封鎖 ChatGPT 爬蟲抓取商品目錄；Walmart/Target 官方合作後，GenAI 推薦流量佔比已是 Amazon 的 3 倍（1.5% vs 0.5%）
- **討論點：** 這代表「要不要讓 AI 爬蟲抓取你的網站」已經是零售業的策略分歧點，不單純是技術問題。

### 4. AI 廣告化的速度遠超預期
- ChatGPT 廣告測試僅 3 個月（2026-02~05），曝光量與見廣告用戶數雙雙成長 **7倍**
- Shopping + Software 兩類合計佔 ChatGPT 廣告近一半
- ChatGPT 廣告地理策略反直覺：避開加州/德州/佛州，主攻中西部/南部「未飽和市場」
- **討論點：** 這跟 W24 週報追蹤的 Agent SDK 計費分池是否是同一套「Anthropic/OpenAI 都在加速變現」敘事的不同面向？值得請 Codex 交叉比對時間軸。

### 5. 整體大盤成長已明顯減速，但「非 Generative AI」類別反而加速
- GenAI App 下載 HoH 成長從 71%（H1 2025）降至 36%（H1 2026）
- 但扣除 Generative AI App 本身，含 AI 關鍵詞 App 的 IAP 營收仍 YoY +40%，達 ~$8B
- 最大推力：Multimedia & Design、Health & Wellness、Jobs & Education，以及短劇 App 帶動的 Movies & TV Shows
- **討論點：** 這代表「AI 泡沫」敘事可能誤導——專用 GenAI App 確實降溫，但 AI 作為「功能」滲透進其他品類的速度反而在加速。這跟我們過去幾週週報「AI 工具疲勞」的觀察是否矛盾？

### 6. 亞洲市場首次出現下載量下滑（13 個季度連續成長後）
- Asia GenAI App 下載 Q1 2026 -3.3%，中東同步下滑
- 拉美、歐洲反而領漲；巴西已超越中國成為下載量第三大市場
- **討論點：** 這跟我們之前完全沒追蹤的「中國/印度 AI App 採用觸頂」現象有關，值得確認是飽和效應還是其他結構性原因（監管、本土替代品競爭等）。

---

## 待 Codex 協助的工作

1. **交叉比對時間軸**：把這份報告的事件（2/26 Anthropic 聲明、2/28 OpenAI-戰爭部協議、ChatGPT 廣告測試 2/9 起、Fable5/Mythos5 6/9 上線+6/12 下架）跟我們 W20~W25 週報已記錄的事件對齊，找出任何矛盾或遺漏的關聯。
2. **數字一致性檢查**：確認本報告內部數字前後一致（如 ChatGPT 解除安裝 +202% 的計算基準、Claude ARPU 成長倍數等）。
3. **補充視角**：以「對 D:\AI_study 週報讀者（關注 AI coding assistant、local LLM、agent 架構）」的角度，指出本報告中哪些數據對於評估「該用哪個 AI 工具」最有實際參考價值。
4. **整合成最終報告**：將討論結果整合進最終版本，存為 `D:\AI_study\sensor_tower_state_of_ai_2026_final.md`。

---

**run log：**
- 草稿撰寫：完成（Claude）
- Codex 討論：待執行
- 最終整合：待執行
