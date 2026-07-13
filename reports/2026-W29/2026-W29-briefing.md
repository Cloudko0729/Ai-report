這是一份為您彙整的本週 AI 新知簡報文件（Briefing Document）：

### 本週 AI 新知整體摘要
本週 AI 領域迎來重大進展，OpenAI 正式推出具備強大代理能力（Agentic capabilities）的 GPT-5.6 模型家族，而 Google 也遭洩漏即將發布具備 200 萬 Token 上下文窗口（Context window）的 Gemini 3.5 Pro [1, 2]。整體 AI 競賽的焦點正在發生轉移，各大廠不再僅追求模型體積的無限制放大，而是更看重經濟效益、模型路由（選擇合適模型處理特定任務）以及打造更便宜且聰明的系統 [3, 4]。此外，開源模型（Open-source models）的強勢崛起正逐漸威脅專有大型模型的商業模式，同時 OpenAI、Anthropic 與 SpaceX 等巨頭的市場價值與影響力，已被評估為超越了過去 25 年的科技公司總和 [5, 6]。

---

### 各主題重點列表

#### 工具與模型 (Tools & Models)
*   **OpenAI GPT-5.6 家族**：推出包含 Sol、Terra 與 Luna 三款不同級別的模型，具備強大的 Agentic capabilities（代理能力），且 API 成本顯著低於競品（如 Claude 的 Fable 與 Opus 模型）[2, 7, 8]。
*   **Google Gemini 3.5 Pro（外洩消息）**：據傳於 7 月 17 日發布，具有全新預訓練基礎。亮點包含 200 萬 Token 的 Context Window、Deep Think（深度思考）推理模式，以及強大的前端與 UI 生成、單樣本（One-shot）遊戲建立能力 [1]。
*   **Nano banana pro（外洩消息）**：傳聞 Google 將推出基於 Gemini 3.5 Pro 基礎的模型，預計直接與 GPT Image 1 競爭圖像原生 AI 生成（Image-native AI generation）市場 [1]。

#### 重大事件 (Events)
*   **OpenAI 關閉 At Last 瀏覽器**：推出僅 9 個月、原旨在挑戰 Google Chrome 的 Web Browser「At Last」宣布終止服務，顯示即便是 AI 巨頭的明星級產品線，也面臨市場接受度的嚴峻考驗 [8, 9]。
*   **AI 巨頭改寫科技史**：報告指出 Anthropic、OpenAI 以及收購了 Cursor 的 SpaceX，這三家公司的發展規模與市場價值，已超越過去 25 年來所有科技公司的總和 [5, 6]。

#### 技術與能力 (Technology)
*   **Autonomous Agent Workflows（自主代理工作流）**：AI 技術正從單純的問答生成，進化為能自主推理、使用工具（Tool use）並實際完成長線工作流程的 Agent（代理）[1]。
*   **Massive Context Window（巨量上下文窗口）**：高達 200 萬 Token 的容量帶來了用例的質變，讓開發者能將整個程式碼庫、法律文獻或多年的企業知識庫一次性放入單一 Prompt（提示詞）中處理 [1]。

---

### 跨來源的共同趨勢分析

*   **趨勢一：從純粹的跑分競爭轉向「Agent-First」（代理優先）與實際執行力**
    綜合兩份來源，AI 產業的發展重點已經轉移。Google Gemini 3.5 Pro 放棄了僅在後端程式碼跑分上爭奪勝負，轉而專注於「自主代理工作流」與視覺互動體驗；而 OpenAI 的 GPT-5.6 也主打強大的代理能力 [1, 2]。這顯示基礎模型（Foundation models）本身已成為基本門檻（Table stakes），未來的真正戰場在於 AI 是否能作為 Agent 實際進行推理、使用工具並完成複雜的工作流程 [1]。
*   **趨勢二：AI 競賽從「追求更大」轉向「注重成本效益」與「適才適用」**
    AI 的競賽模式正在改變，不再單純比拼誰的模型最大、最新，而是轉向更便宜、更聰明的系統（Cheaper, smarter systems）[3, 4]。如同 Perplexity CEO 所強調的，未來的核心產品價值在於「系統能為每個特定任務自動選擇合適的模型」（例如殺雞焉用牛刀，小 Bug 使用低成本模型即可）[3, 4]。同時，Open-source models（開源模型）預期將能處理大部分的 AI 使用場景，這對依賴高昂訂閱與 API 費用的巨型模型供應商將帶來巨大的經濟壓力 [5]。