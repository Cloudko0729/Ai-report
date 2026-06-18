## Build and Run Llama.cpp with CUDA Support (Updated Guide)

這是一段為您準備的週報摘要：

本週教學介紹了如何從零編譯支援 CUDA 的 **Llama.cpp** [1, 2]。以下為三個核心重點：

1. **本地編譯 Llama.cpp**：詳細解說如何使用 Git clone 下載原始碼，並透過 **CMake** 搭配 Visual Studio 環境工具進行本地建置，以獲得完整的 GPU 加速支援 [3-5]。
2. **GGUF 模型應用與測試**：示範從 **Hugging Face** 下載輕量化的 **GGUF** 格式模型，使用命令列參數開啟對話模式（`-cnv`），並利用 `-ngl` 指令將層數卸載至 GPU 提升生成速度 [6-9]。
3. **純聊天替代方案推薦**：**Llama.cpp** 極度適合開發者作為後端整合使用；但若用戶僅需要簡單好用的 AI 對話機器人，強烈推薦直接下載免安裝的 **KoboldCPP** [10, 11]。

## Cursor 3 Changes Everything for Agentic Coding

本週新知聚焦於 **Cursor 3** 的重大更新，此次改版專為 Agentic Coding 打造，徹底顛覆傳統的開發體驗：

* **全視角 Agent 工作區**：全新極簡介面支援同時跨專案運行多個 **Agent**，並內建瀏覽器供 AI 自動進入網頁測試修復成果，甚至能直接處理建立 PR 等 CI/CD 流程 [1-3]。
* **高效能 Composer 2**：採用全新的 **Composer 2** 模型，不僅推論速度極快，且 API 成本遠低於同級別的頂規模型 [4]。
* **Local 與 Cloud 無縫協作**：支援將本地端 (**Local**) 任務一鍵移交至雲端 (**Cloud**) 執行，即使電腦關機 AI 也能持續開發；同時新增 Marketplace 讓開發者輕鬆擴充 **MCP servers** 與各式 Skills [5-7]。

## Cursor 3 is Not What You Think

本週關注 **Cursor 3.0** 的重大更新，其開發環境已進化為 **Agents** 的編排層（orchestration layer），大幅提升自動化開發效率 [1, 2]。

*   **支援多模型 Multi-Agent 並行**：打破單一 **LLM** 限制，開發者可依任務需求，同時運行多個由 Claude、Gemini 或 OpenAI 等不同模型驅動的 **Agents** [3, 4]。
*   **視覺化 Design Mode**：專為前端與設計優化，能直接點選 UI 元素並自動帶入程式碼與截圖作為上下文（context），實現精準的針對性修改 [5-7]。
*   **Cloud Agents 與 GitHub 整合**：支援將 **Agents** 部署至雲端環境徹夜運行，甚至可透過 **Slack** 遠端下達指令；所有本地或雲端的修改皆能一鍵建立並合併 **PR** [2, 8, 9]。

## GPT Realtime 2: OpenAI Realtime API Explained: GPT Realtime 2, Voice AI, And Live Translation

這是一段適合週報的摘要：

OpenAI 全新推出的 GPT Realtime API 捨棄了傳統的 Cascade Pipeline，改採 End-to-end Multimodal Architecture 直接處理原始音訊，大幅提升語音互動的自然度與流暢性 [1, 2]。

**本週重點摘要：**

*   **深度推理與低延遲**：GPT Realtime 2 內建了 GPT-5 等級的 Chain of Thought reasoning [3]。開發者可透過調整 `reasoning effort` 參數，在智慧運算與低於 400 毫秒的低延遲（Latency）之間取得最佳平衡 [4]。
*   **超大記憶體與成本優化**：模型具備 128K Token 的 Context Window，能記住數小時的語音對話 [5]。針對高昂的音訊處理成本，開發者必須善用 Text Caching 來快取系統提示詞，以避免運算成本失控 [6, 7]。
*   **同步翻譯與平行工具**：全新的 GPT Realtime Translate 提供無需等待的同步翻譯，並透過 Dynamic Voice Adaptation 還原說話者的真實語氣 [6, 8]；系統同時支援 Parallel Tool Execution，能一次觸發多個後端資料庫與 API [4]。

## How to Install Llama.cpp on Windows 11 (CUDA 13 & RTX 50-Series Guide)

本影片教學示範如何在 Windows 11 系統上，針對最新 RTX 50-Series 顯示卡安裝並編譯支援 CUDA 13 的 Llama.cpp [1-3]。

重點摘要如下：
1. **環境建置**：需下載並安裝 CUDA Toolkit、CMake 與 Visual Studio Build Tools，並透過 `vcpkg` 安裝必要套件及設定環境變數 [1, 2, 4]。
2. **編譯設定**：使用 CMake 進行編譯配置，需特別指定 Blackwell 架構參數（`CMAKE_CUDA_ARCHITECTURES=100`）與正確的 CUDA 路徑 [2, 3]。
3. **本地推論**：編譯完成後，可至 Hugging Face 下載模型，並透過 `llama-cli.exe` 執行本地端的 AI 推論與生成 [3, 5]。

## Introducing gpt-realtime in the API

這是一段為您準備的週報摘要：

*   **模型發布**：OpenAI 推出全新原生端到端語音模型 **GPT Realtime** 及 **Realtime API**，具備超低延遲、豐富情感展現與無縫多語切換能力 [1, 2]。
*   **核心升級**：模型顯著強化了 **Instruction Following** 與 **Function Calling** 表現，並首度支援 **Image Input**（圖像輸入）；API 亦新增 SIP 與 **MCP** 支援 [3-6]。
*   **實際應用**：T-Mobile 導入此 API 打造高擬真 AI 語音助理，能靈活應對顧客隨機提問與情緒，實現自然流暢的真人級客服體驗 [7-9]。

## UPDATE: Anthropic's New 'Dreaming' Feature Makes Claude Dangerously Smart

Anthropic 為 Claude 推出全新「Dreaming」功能，賦予 AI 長期記憶與自我反思能力，大幅改變 AI 代理 (Agents) 的運作方式 [1, 2]。

本週三大重點：
1. **「Dreaming」與長期記憶 (Long-term memory)**：Claude 能在背景非同步回顧多達100個對話紀錄，提取模式並清除過時的記憶腐敗 (Memory rot)，建立高質量記憶結構 [1, 3]。
2. **自動優化與適應**：無需重新訓練基礎模型 (Foundation model)，AI 即可從經驗中自我提升。法律 AI 測試案例顯示，其任務完成率激增近6倍 [2, 4]。
3. **「Outcomes」與多代理協作 (Multi-agent orchestration)**：Claude 現具備自我評分與修正功能，且主代理能將任務拆解並指派給子代理平行處理，實現強大自主認知迴圈 [4, 5]。

## [vLLM Office Hours #48] vLLM Project and Tool Calling Update - April 30, 2026

以下為適合週報的摘要：

* **vLLM 0.20 重大更新**：預設升級支援 PyTorch 2.11 與 CUDA 13.0 [1]。新增對 **DeepSeek V4** 的首發支援（包含百萬 **context** 處理與極致 **KV cache** 壓縮）[2-4]，並推出全新互動式模型部署指南 **recipes.vllm.ai** [5, 6]。
* **深入 Tool Calling 架構**：詳細解析 **Tool Calling** 的三大核心：LLM、**Chat Template** 與 **Tool Call Parser** [7]。團隊致力解決設定不符所導致的隱性失效，並透過導入 **Structured Outputs** 與評測框架（如 BFCL）來確保輸出的準確性 [8-10]。
* **完善 Agentic 工作流 API**：vLLM 現已原生支援 **Anthropic Messages API** [11, 12]。開發者無需額外串接代理伺服器（Proxy），即可讓開源模型順暢驅動 **Claude Code** 與 **Open Code** 等複雜的 **Agent** 應用 [12, 13]。

## 🎙️Top 5 new VLLM features 2026! with Simon Mo @ 𝗥𝗮𝘆 𝗦𝘂𝗺𝗺𝗶𝘁

這是一段為您整理的 vLLM 最新進展週報摘要：

本週為您帶來 Ray Summit 中 vLLM 專案負責人 Simon Mo 所分享的最新進步 [1]。vLLM 持續鞏固其作為頂尖開源 AI **inference engine** 的地位，透過底層架構與生態系的全面升級，大幅提升效能，三個核心重點如下：

*   **API 與模型支援擴充**：除了原有的 OpenAI API，現已支援 Anthropic API 與視覺語言模型 [1, 2]。目前支援超過 200 種模型架構，並提供如 DeepSeek OCR 等新模型的 **day zero** 支援 [2, 3]。
*   **核心 Engine 無縫升級**：團隊已完成 **v1** 核心引擎的全面重構，使用者在完全不需修改程式碼的狀態下，即可獲得 **2x** 的效率提升 [3]。
*   **硬體 Plug-in 與分散式擴展**：透過全新的 **plug-in** 系統，輕鬆支援 Google TPU、Intel Gaudi 等多種加速器晶片 [4]，並與 NVIDIA Dynamo、Red Hat 等夥伴合作，實現大規模叢集的 **scale out** 部署 [5]。
