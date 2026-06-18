## Anthropic Launches Claude Design and Opus 4.7

本週 **Anthropic** 推出了兩項重大更新：**Claude Design** 與 **Opus 4.7** 模型 [1]，以下為本週報重點摘要：

* **推出 Claude Design**：這是一款強大的 AI 視覺設計與白板工具，能快速生成網頁、簡報及社群素材，由前 Instagram 創辦人主導，被視為 **Figma** 的強大競爭對手 [2-4]。
* **Opus 4.7 導入 Model Router**：新模型加入了模型路由（Model Router）機制，能自動判斷問題難易度來切換適合的底層模型，藉此平衡運算成本與效能 [5]。
* **快速根據回饋優化**：針對專家早期測試的回饋，**Anthropic** 迅速優化了 **Opus 4.7** 的自適應思考能力，大幅增加觸發深度思考與網路搜尋的頻率，顯著提升非程式編寫任務的輸出品質 [6, 7]。

## Build Better Agent UX: Streaming Progress, Status, and File Ops with LangChain

這是一段為您準備的週報摘要：

本週 LangChain 釋出關於優化 **Agent UX** 的技術教學，展示如何處理耗時較長的 **tool call** [1]。

* **提升 UI 響應性**：打破傳統單一載入指示器的限制，將後端工具執行的即時進度串流至前端，大幅優化使用者體驗 [1, 2]。
* **自訂串流事件 (Custom Stream Events)**：透過工具運行環境中的 `config.writer` 函數，開發者可向前端發送帶有類型標籤及 `tool_call_id` 的自訂進度與狀態事件 [3]。
* **前端接收與動態渲染**：前端透過 `use_stream` hook 內的 `oncustom` 處理器接收事件，結合 TypeScript 型別驗證，即可同步渲染多個工具的即時進度卡片 [4, 5]。

## How to Use GitHub Copilot Agent Mode (Full Guide 2026)

這份來源介紹了如何上手 **GitHub Copilot Agent mode**，以下為適合週報的三個重點摘要：

1. **導覽與核心定位**：說明如何在 GitHub 導覽列中找到 **Copilot Cloud Agent**，其主要功能是處理重複性任務與設定，讓開發者專注於高階決策 [1]。
2. **功能邊界與安全規範**：建議透過官方文件了解 Agent 的能力範圍、應用場景及安全護欄（Guardrails），並特別提醒避免在提示詞中輸入機密或敏感資料 [1]。
3. **權限限制與介面提示**：Agent 的使用權限取決於目前的訂閱方案，而介面上的 **Spark** 圖示即代表 AI 輔助功能的快捷入口 [1]。

## What's new with the Copilot coding agent | GitHub Checkout

本週 **GitHub Copilot coding agent** 最新重點整理：

* **Agents Panel 與 MCP 整合**：新增 **agents panel** 讓開發者更輕鬆指派與追蹤任務 [1]。系統預設啟用 **Playwright** 與 **GitHub MCP servers**，賦予代理進行網頁測試、截圖分享以及讀取專案 issue 的強大能力 [2, 3]。
* **高效處理 Tech Debt**：此代理工具非常適合用來清理技術債（例如重構程式碼或升級 **dependencies**），也可協助開發者預先完成 70% 至 80% 的初期功能建置 [3-5]。
* **方案放寬與未來藍圖**：現已全面開放給所有付費方案使用，每次建立 **PR** 僅需扣除一次 **premium request**（將消耗 **GitHub actions** 分鐘數） [5, 6]。未來預計推出 **Public API**，並支援自動修復 **GitHub actions** 構建失敗等新功能 [6, 7]。
