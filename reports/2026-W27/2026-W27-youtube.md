## Claude Sonnet 5 IS OUT & ITS HORRIBLE! Worst Model By Anthropic EVER? (Fully Tested)

Anthropic 最新推出的 **Claude Sonnet 5** 號稱具備強大的 Agentic（代理）與工具使用能力，但實測結果卻不如預期 [1, 2]。以下為本週實測的三大重點：

* **代理能力與前端表現落差**：雖然在 Agentic Coding 等 benchmarks 成績亮眼，並能生成基本的 Mac OS 介面，但複雜的前端設計與 SVG 繪圖表現極差，甚至不如 GLM 5.2 [1-4]。
* **Token 消耗效率極低**：帳面定價雖具吸引力，但因改用 Opus 4.7 tokenizer，執行時會消耗更多 tokens，實際成本並未真正降低，被評為極度 token inefficient 的模型 [5-7]。
* **建議維持使用 Opus 4.8**：考量到兩者極小的真實價差與顯著的效能落差，實測結論強烈建議跳過 Sonnet 5，繼續將 **Opus 4.8** 作為日常工作的主力模型 [6-8]。

## Claude Sonnet 5 Just Dropped (I have to be honest...)

Anthropic 最新發布 **Claude Sonnet 5**，該模型未追求技術極限，而是專注於降低中階任務成本並提升基礎能力，成為政府嚴格監管下少數成功推出的模型 [1, 2]。

**三個重點：**
1. **高性價比與實用性**：效能雖略遜於 **Opus 4.8** 但大幅超越 **Sonnet 4.6**。它擅長 **tool use** 與長期自主運行，極適合應用於 **co-work** 及 **sub-agents** [1, 3]。
2. **限期價格優惠**：上市初期定價親民（輸入 $2 / 輸出 $10 每百萬 tokens），2026年8月31日後將調漲至 $3/$15，是建立系統底層（plumbing）的低成本好選擇 [3, 4]。
3. **為合規妥協安全能力**：為避開政府對 **cybersecurity**（網路安全）的審查與阻擋，官方刻意削弱了該模型在漏洞利用上的能力，以確保其能順利發布 [2, 5]。

## Claude Sonnet 5: No Hype Full Breakdown & Testing

Anthropic 最新推出 **Claude Sonnet 5**！經由實測，它能以一半的價格提供約 95% **Opus 48** 的效能[1, 2]。以下是本次實測的三大重點：

1. **Coding (程式開發)**：複雜專案 (如遊戲開發) 仍由 Opus 48 勝出，但 Sonnet 5 在 **Landing Page** 設計上表現媲美 Opus 48，且成本大幅降低[3, 4]。
2. **Agentic Use (代理任務)**：Sonnet 5 在中低難度的電腦操作與搜尋任務上表現優異，成為高性價比首選，但極高難度任務仍依賴 Opus 48[5, 6]。
3. **Knowledge Work (知識工作)**：Sonnet 5 在 **Slide Deck** (簡報) 設計與特定寫作測試 (如 YouTube 腳本撰寫) 上，表現甚至超越了 Opus 48[7]。
