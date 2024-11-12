# CS 194/294-196 (LLM Agents) - Lecture 7, Nicolas Chapados and Alexandre Drouin

## 課程筆記

**Lecture 7: Agent Systems in Enterprise Context**
=====================================================

### Introduction

* **NICOLAS CHAPADOS**: We're thrilled to be here.
* **Context**: Midpoint of the lecture series, focusing on agent systems in enterprise context.

### Building Blocks for Agent Systems

* **Reasoning and Tool Use with AI Agents**:
	+ Understanding how agents can be used in enterprise context
	+ Focusing on use cases, users, roles, work, and deployment context

### Enterprise Context and Workflows

* **ServiceNow**: A global company (25,000 employees) that builds a platform to automate enterprise workflows.
* **Workflows**: The bread and butter of ServiceNow's business.
* **Platform**: Used in areas like IT, service management, human resources, customer support.

### Opportunities for AI Agents

* **Automating Everyday Issues**:
	+ Processing tickets for IT help desk
	+ Requesting new laptops to be shipped
	+ Huge opportunities for AI agents to automate partly some of this work

### Research and Development

* **ServiceNow Research**: Our team works on agents, focusing on understanding use cases, users, roles, work, and deployment context.

**LLM-Powered Agents**
=====================

### Introduction

*   We have multiple sub-teams working on various aspects of agent development.
*   These teams also consider other layers of the stack, such as:
    *   Training and fine-tuning foundation models (e.g., StarCoder model)
    *   Ensuring AI trustworthiness, governance, safety, security, and practical concerns

### Agenda for Today's Lecture

1.  **Background**
    *   Brief overview of AI agents
    *   Explanation of vocabulary and terminology
2.  **Enterprise Workflows**
    *   Discussion on the challenges and current work in businesses today
3.  **API Agents**
    *   Overview of API agents and their architectures
4.  **TapeAgents Framework**
    *   Introduction to the new open-source framework for developing and optimizing agents
5.  **Web Agents**
    *   Presentation by Alex on web agents, including:
        +  Building simple web agents
        +  Measuring performance and improving web agents in a principled way
        +  Tooling for building, developing, and optimizing web agents
6.  **Conclusion**
    *   Discussion on the potential of agents in the workplace and large-scale transformations they could bring

### Key Concepts

*   **LLM-Powered Agents**: Agents that utilize Large Language Models (LLMs) to operate.
*   **Autonomy**: The ability of an agent to plan, take action, receive feedback, and execute goals given by a human user.

**LLM Agents**
================

### 定義與類型

*   **LLM (Large Language Model) agents**: 利用大規模語言模型的能力，能夠執行複雜任務
*   **API Calling Agent**: 使用 API 來交換文字資訊
*   **Web Agent**: 能夠使用網頁，點擊按鈕、填寫表單等

### 特徵與優缺點

#### LLM Agents

*   **訓練資料**: trained on a large fraction of the internet
*   **知識範圍**: 有能力執行多種任務，包括軟體操作
*   **優點**: 能夠利用已經有的知識來完成任務
*   **缺點**: 可能會因為訓練資料的限制而無法處理某些任務

#### API Calling Agent

*   **功能**: 使用 API 來交換文字資訊
*   **優點**: 能夠快速地執行特定的任務
*   **缺點**: 只能夠使用已經定義好的 API

#### Web Agent

*   **功能**: 能夠使用網頁，點擊按鈕、填寫表單等
*   **優點**: 能夠處理複雜的任務，並且能夠記住一些資訊
*   **缺點**: 可能會因為網頁的變化而無法正常執行

**工作流程自動化**
================

### 0. 問題描述

*   Jon 對公司內部知識庫有存取權。
*   Jon 的 IT 帕台發出了一個案件，該案件被指派給 Sandy。

### 1. 解決方案

#### 1.1 查找已經存在的知識庫文章

*   Sandy 檢查是否有相關的知識庫文章。
*   如果沒有找到相關文章，她會繼續進行下一步驟。

#### 1.2 查找類似的案件

*   Sandy 檢查是否有以前的案件類似於目前的問題。
*   如果找到類似的案件，她會根據該案件的解決方案進行處理。

#### 1.3 修改存取控制

*   Sandy 檢查 Jon 的存取控制權限。
*   如果 Jon 沒有適當的存取控制權限，Sandy 將修改存取控制權限。

### 2. 使用 AI 助手

*   Sandy 可以使用公司內部的新一代生成式 AI 能力來幫助她處理案件。
*   這個 AI 能力可以幫助她進行事件摘要、寫解決方案筆記和關閉案件。

### 3. 結論

*   即使有 AI 助手，工作流程仍然需要許多人工步驟。
*   這種情況在企業中非常普遍，每天都有數百萬個類似的事件發生。

### 4. 工作流程自動化的進展

*   在過去幾年中，企業工作流程自動化的技術已經從高度程式化、低自動化度到使用 AI 的更高自動化度。
*   這些新技術包括建議系統、對話流程和現在的代理工作流程。

### 5. 未來展望

*   在未來，代理工作流程將是企業工作流程自動化中最有前景的領域。
*   這種技術可以幫助企業自動化大量低價值、低頻率的任務。

**低值、低量企業自動化**
=====================================

### 不值得投資的領域

*   **低值、低量** 的工作流程或程序
*   已經有人解決了高價值、高頻率的問題

### 企業自動化的挑戰

*   **低成本、低效率** 的自動化工具
*   **重複性高、可預測性高** 的工作流程
*   可能已經有 **低代碼** 或 **無代碼** 的環境或機器人流程自動化 (RPA) 處理

### 個別工作的挑戰

*   **難以被程式化或自動化**
*   每次都不同,難以被重覆使用
*   例如: 
    *   自動發送推文或回應郵件
    *   更新客戶關係管理系統 (CRM)
    *   組織會議

### 代理程式的潛力

*   **解決難以被程式化或自動化** 的工作
*   個別工作雖然小,但在整體中代表大量的工作量
*   可能有助於改善工作效率和流程

**Conference**
================

### Google Maps Navigation

*   [16:21] It's finding the San Jose Convention Center
*   [16:25] and this is what it is entering into Google Maps
*   [16:29] now to figure out the way to get from the NVIDIA headquarters to the San Jose convention center.

### Interaction with Agents

*   [16:36] This is an example of the kind of interaction that we soon will be getting or that we hope we should be getting with our agents.
*   [16:44] as systems that are allowed to ask more questions to humans but that have some smarts in terms of planning and replanning of their own.

### API Agents

#### Architecture

*   We start with an LLM agent that is able to emit some actions, and those actions are sent to an environment.
*   The environment sends back observations back to the LLM agent.
*   The agent has access to some short-term memory. So what have been the past actions taken and the past responses from the environment.

#### Planning Processes

*   It also has access to some planning processes, so things like react and so on.
*   There are many different strategies that have been proposed. We're not going to get too much into those today.

#### Tools and Long-term Memory

*   And of course, for agents to be useful, it has to access some tools and the tool there can be quite varied, including simple calculations, running code, accessing the web and so on.
*   And some more advanced agents also have the ability to synthesize new tools and those can be stored in some kind of long-term memory.

### Software Framework

#### Need for a Right Framework

*   Just like it would be crazy for anyone today to try to program machine learning algorithms from scratch. Everybody uses PyTorch because it's so much faster. It's so much easier.
*   We want to have the right framework to build agents.

#### TapeAgents Framework

*   We introduce this framework called TapeAgents just a couple days ago. In fact, the QR code is the link to the resources. All of that will be given again at the end, don't worry.
*   And what we're trying to accomplish with tape agents that is to get a little bit of the best of both worlds.

#### Holistic Agent Development

*   On the one hand, we have frameworks that really address the need for the software engineering part of agents. We want to be able to specify those agents to a very fine degree of granularity, to

**TapeAgents Framework**
=======================

### 重要概念

*   **Tape**: 一個統一的抽象, 是一個日誌或記錄系統, 儲存所有代理在系統中的思想和行為。
*   **Prompt Optimization**: 這是對LLM進行優化以改善代理性能的一種技術。

### TapeAgents Framework 的特點

#### 1. 具有預先組建的組件
#### 2. 支援並發性和串流功能
#### 3. 可與 LLM 整合
#### 4. 支援 LangGraph、AutoGen 等框架
#### 5. 提供優秀的代理開發工具

### TapeAgents Framework 的目標

*   **最佳化**: 提供一個能夠同時進行代理開發和優化的框架
*   **促進**: 透過 Tape 的統一抽象, 提高代理性能並減少開發時間

### TapeAgents Framework 的執行模型

#### 1. Tape 的儲存和處理

*   **Tape**: 儲存所有代理在系統中的思想和行為
*   **Agent B**: 可以讀取整個 Tape 的歷史, 選擇執行特定節點

### TapeAgents Framework 的優勢

#### 1. 提供一個統一的抽象
#### 2. 支援多代理系統
#### 3. 提高代理性能和開發效率

**抽象觀點**
================

### **小節**

*   **[22:53] 小節**: 決定如何觸發 LLM 的小節。
*   **[22:57] 代理人**: 可以有多個或少於一個節點。

### **執行模型**

*   **[23:01] 執行模型**: 由代理人決定內部結構。
*   **[23:07] 節點**: 呼叫 LLM、提出幾個想法或行動、添加到帶子中。
*   **[23:18] 角色**: 呼叫環境執行未處理的動作、取得回應和循環。

### **模組化**

*   **[23:38] 多代理人**: 每個代理人可以委派工作給子代理人。
*   **[23:46] 模組化**: 使結構變得非常靈活。

### **功能**

*   **[23:52] 帶子**: 作為資料的帶子。
*   **[24:03] 完全審計和偵錯**: 可以進行完整的審計和偵錯。
*   **[24:09] 算法**: 使用帶子作為輸入、進行循環提示優化。

### **簡單範例**

*   **[24:41] 代理人系統**: 具有兩個代理人的系統。
*   **[25:05] 問題回答助手**: 問題回答助手和子代理人。
*   **[25:27] 執行模型**: 使用執行模型結合代理人。

### **帶子的功能**

*   **[25:39] 互動記錄**: 記錄代理人的內部思維、推理跡蹤和環境回應。
*   **[26:00] 帶子**: 在實踐中，帶子是非常複雜的。

### **簡單範例**

*   **[25:51] 代理人系統**: 可以通過入門筆記重現範例。

**GREADTH Conversational Agents**
=====================================

### 重要概念

*   **GREADTH**: Attributes for measuring conversational agent quality, including groundedness, non-hallucination, truthfulness, responsiveness, accuracy, discipline, transparency, and helpfulness.
*   **LLAMA**: A large language model architecture.

### Case Study: Complex Form Filling
--------------------------------------

#### Objective

*   Create a cost-effective conversational agent that can provide high-quality user interaction for filling out complex forms.

#### Methodology

1.  Train a complicated agent on LLAMA 3.5, 3.14, and 5 billion parameter models.
2.  Record execution traces as discrete tapes.
3.  Fine-tune a LLAMA 8 billion parameter model to recover the performance of the larger parent model.

#### Results

*   Achieve substantial success in fine-tuning the LLAMA 8 billion parameter model.
*   See significant cost savings compared to running a million conversation turns with the original large model.

### GREADTH Attributes
----------------------

*   **Groundedness**: The agent's ability to stay focused on the task at hand and avoid hallucinations.
*   **Non-hallucination**: The agent's ability to provide accurate and relevant responses without making things up.
*   **Truthfulness**: The agent's commitment to telling the truth and providing accurate information.
*   **Responsiveness**: The agent's ability to respond quickly and efficiently to user queries.
*   **Accuracy**: The agent's ability to provide accurate and relevant responses.
*   **Discipline**: The agent's ability to stay on track and avoid distractions.
*   **Transparency**: The agent's commitment to being clear and transparent in its interactions with users.
*   **Helpfulness**: The agent's willingness to assist users and provide helpful information.

**TapeAgents**
================

### 概念介紹

*   **Quality Measure**: 使用先前引入的高品質計量方法。
*   **Agent Loop**: 代理循環，包括感知、決策和行動。

### TapeAgents 的優點

*   **成本效益**: 使用 TapeAgents 可以在不犧牲性能的情況下大幅降低成本。
*   **可擴展性**: TapeAgents 可以應用於各種代理框架中。

### Web Agents
-----------------

### 概念介紹

*   **Web Agent**: 一種能夠與使用者互動的代理，無需 API 支持。
*   **Agent Loop**: 代理循環，包括感知、決策和行動。

### Web Agents 的挑戰

*   **理解目標**: 需要了解使用者的目標和需求。
*   **環境感知**: 需要能夠感知網頁環境的變化。
*   **決策能力**: 需要能夠做出適當的決定。

### TapeAgents 與其他代理框架比較
--------------------------------------

| 框架 | TapeAgents |
| --- | --- |
| 成本效益 | >>>>>>>> |
| 可擴展性 | >>>>>>>> |

備註：以上內容僅為筆記用途，具體內容可能與原文有所不同。

**基本網頁代理人**
================

### 定義和挑戰

*   **長期規劃**: 由於目標結果通常不在當前頁面，需要轉換、導航菜單等。
*   **執行行動**: 即使制定了計畫，也需要正確執行行動。

### 建立基本網頁代理人

#### 步驟 1:構建提示

*   **任務描述**: 描述目標任務
*   **觀察**: 提供網頁的 HTML 內容
*   **行動空間**: 定義代理人可以執行的行動（如點擊控制項、填寫表單等）

#### 步驟 2:使用 LLM

*   將提示提供給 LLM
*   請求 LLM 根據觀察和任務描述產生行動

#### 步驟 3:執行行動

*   使用 Python 和 Playwright 或 Selenium 等工具在瀏覽器中執行代理人生成的行動

### 範例

*   **輸入 Enola**: 在表單中填寫 Enola，然後點擊提交
*   **GPT-4 基礎代理人**: 使用 GPT-4 產生代理人，可以根據提示完成基本任務

**GPT-4與React-style Prompt**
=====================================

### 基礎概念

* **GPT-4**:基於GPT-4的模型，具有React-style提示功能。
* **React-style Prompt**:一個簡單的提示，用於觸發GPT-4進行思考和行動。

### 範例應用

* **填寫費用報告**:使用GPT-4填寫費用報告，模擬實際情況。
* **自動化任務**:通過GPT-4來自動化任務，例如填寫表格、點擊提交等。

### 限制和挑戰

* **脆弱性**:這種模型現在很脆弱，容易被破壞或竊取。
* **可靠性**:需要在實際情況下工作時，需要確保其可靠性。
* **速度**:GPT-4的執行速度較慢，目前只能通過加速來顯示。

### 基準測試

* **簡單網頁任務**:建立基於簡單網頁任務的基準測試。
* **真實世界網站基準測試**:基於真實世界網站的基準測試，包括追蹤人們在網站上的行為。

### 未來展望

* **進一步發展**:基於GPT-4和React-style Prompt的模型將繼續發展。
* **更好的可靠性和速度**:未來將嘗試改善其可靠性和執行速度。

**Trace-based Data Sets**
==========================

### 限制與問題

*   **Alternative Solutions**: 不考慮可能存在的替代解決方案。
*   **Memorization Risk**: 存在風險被 LLMS 記住並使用。

### 新型基準

*   **Murthy et al. 的基準**：使用 LLM 生成隨機行動，並回顧後標記目標。
*   **優點**：
    *   可以產生數千個樣本而不需要人工標注。
    *   可用於評估和微調。

### Live Benchmarks

#### 基於結果的基準

*   **評估基準**：根據最終結果進行評估。
*   **優點**：
    *   可以考慮替代解決方案。
    *   降低了記憶風險，因為不儲存行動序列。

#### 例子

*   **WebArena**: 基於軟件任務（如 Reddit 或 GitLab），評估代理能否達成目標。
*   **Visual WebArena**: 視覺化版本的 WebArena。

### 其他基準

*   **問答基準**：檢查代理是否返回正確答案，而不是檢查步驟序列。

**實際的網路**
================

### **優點**

*   可以支援非開源的網站
*   不需要在本地端主機
*   可靠性較高

### **缺點**

*   可能有網路問題
*   需要連上網才能進行測試

**WorkArena**
=============

### **定義**

*   是一種遠端主機的測試工具
*   基於ServiceNow產品開發
*   600個工作相關任務

### **功能**

*   可以進行簡單到複雜的任務
*   可以模擬真實的工作流程

### **運作方式**

*   使用developer instances來提供測試環境
*   使用back end APIs來驗證測試結果

**WorkArena**
================

### **什麼是 WorkArena?**

*   **開放源碼**: WorkArena 的基礎是開放源碼的基礎, 但 ServiceNow 的產品不是。
*   **真實應用**: WorkArena 是一個真實的產品, 人們在使用它時可以看到各種任務。

### **WorkArena 的任務類型**

#### **簡單任務 (Level 1)**

*   **範例**: GPT-4 解決一些簡單任務, 如購買 Apple Watch、瀏覽儀表板、填寫表格等。
*   **特點**: 這些是 WorkArena 中最簡單的任務。

#### **困難任務 (Level 3)**

*   **範例**: GPT-4 解決一個更困難的任務, 如處理一張票, 需要在儀表板中找到庫存最低的物品並重新補充。
*   **特點**: 這個任務需要多步驟, 包括查詢知識庫、瀏覽儀表板等。

### **WorkArena 的能力**

#### **規劃和問題解決**

*   **範例**: GPT-4 解決一個任務, 需要根據員工的忙碌程度重新分配工作。
*   **特點**: 這個任務需要分析資料並做出決定。

**Workload Balancing**
=====================

### 重要概念

*   **WorkArena**: 一個基於真實工作流程的基準測試
*   **Scheduling with Constraints**: 基於限制的排程
*   **Sophisticated Memorization Tasks**: 高度複雜的記憶任務
*   **Critical Thinking**: 思維嚴肅

### 重要概念列表

1.  **Workload Balancing**
2.  **Scheduling with Constraints**
3.  **Sophisticated Memorization Tasks**
4.  **Critical Thinking**

### WorkArena 基準測試

#### WorkArena L1

*   人類評估結果: 94% 成功率
*   最好代理機器人: 42.7% 成功率

#### WorkArena L2

*   人類評估結果: 94% 成功率 (無法提供)
*   最好代理機器人: 0 成功率

#### WorkArena L3

*   人類評估結果: 94% 成功率
*   最好代理機器人: 0 成功率

**BrowserGym**
================

### 什麼是 BrowserGym?

*   **標準化的觀察空間**: 提供標準化的觀察空間，讓使用者可以輕鬆地建立和比較不同網頁代理。
*   **多種觀察模式**: 支援多種觀察模式，包括 HTML、Accessibility Tree、螢幕截圖和聊天盒。

### BrowserGym 的功能

*   **標準化的行動空間**: 提供標準化的行動空間，使使用者可以輕鬆地建立和比較不同網頁代理。
*   **人工評估**: 支援人工評估，讓使用者可以將任務分配給人工評估員。

### BrowserGym 的優點

*   **統一評估平台**: 提供一個統一的評估平台，使使用者可以輕鬆地比較不同網頁代理。
*   **易於使用**: 支援 pip 安裝和 QR 碼訪問，讓使用者可以輕鬆地開始使用。

### 相關工具

*   **AgentLab**: 另一個用於建立網頁代理的工具。

**Web Agent 架構**
================

### **簡介**

*   提供簡單的建置塊和工具來建立 Web 代理。
*   支援 debug、性能優化和大規模實驗。

### **AgentXRay**

*   **功能**: 
    *   顯示代理執行過程中的螢幕截圖
    *   顯示網頁的存取性樹狀結構
    *   顯示代理的推理跟蹤和動作記錄
    *   提供時間線來顯示執行過程中的耗時情況

### **AgentLab**

*   **功能**:
    *   提供標準化的觀察記錄
    *   支援儲存和共享這些記錄
    *   支援建立領先榜單並檢查結果是否仍然有效

### **結合 BrowserGym**

*   **優點**: 
    *   提供標準化的觀察記錄
    *   支援儲存和共享這些記錄
    *   支援建立領先榜單並檢查結果是否仍然有效

**Web Agent Challenges**
=======================

### **Distributed Trace Collection**

*   [55:06] and public repositories to store traces
*   Potential for distributed trace collection
*   Everyone can help gather traces of web agents acting on the open web
*   Collect a big repository of traces for fine tuning and making better agents in the future

### **Challenges of Web Agents**

#### Long Context Understanding

*   Huge websites with tens of thousands to hundreds of thousands of tokens
*   Accessibility trees are supposed to be shorter than HTML, but still huge observations
*   Small amount of relevant information in those contexts, challenging to pick out correctly

#### Long Term Planning

*   Hard to reason about pages without information on what's two or three pages away
*   Intuition for navigation and search is not applicable to LLM agents
*   Work needs to be done in this space, e.g., Murthy et al. paper on collecting traces of random actions at a large scale

#### Learning and Adaptability

*   Need to learn from observation, demonstrations, and mistakes
*   Some work in this direction, e.g., Agent Q using Monte Carlo tree search and DPO for fine tuning agents and inference time search
*   Multi-modality is very important, e.g., visual web arena benchmark proposes tasks that can't be solved without vision modality

#### Cost and Efficiency

*   As mentioned earlier, cost and efficiency are important considerations for web agents

**Web Agents**
================

### 問題點

*   **速度**: 我們展示的視頻被加速了很多。
*   **效率**: 我們需要使其快速且有效率。

### 方向

#### 1. **縮小上下文大小**

*   縮小上下文大小可能是一個方向。

#### 2. **使用回收技術**

*   可以使用回收技術來只取出相關的元素。
*   這樣可以提高效率。

#### 3. **多代理架構**

*   可能存在多代理架構，例如日期選擇器代理。
*   這種架構可以使系統更加高效。

#### 4. **微調小型LLM**

*   微調小型LLM可能是一個選擇。
*   這樣可以提高系統的穩定性。

### 安全

*   **安全**: 安全是非常重要的一點。
*   我們不能讓代理被輕易竊取或操控。
*   目前的代理已經通過測試，證明其穩定性。

### 未來展望

*   **未來展望**: AI代理將會改變工作的本質。
*   這是一個巨大的挑戰，但也是一個機會。

**AI Agents 在工作流程中的作用**
=====================================

### **前言**

* AI agents 可以幫助 Sandy 的工作效率提高。
* AI agents 會先嘗試解決問題，減少人工干預。

### **自動化工作流程**

* AI agents 會嘗試解決問題，並提供步驟。
* 步驟包括：
	+ 找到 Jon 的權限。
	+ 修正知識庫文章的權限。
	+ 將 Jon 的權限與知識庫文章的權限對齊。
* 人工確認後，AI agents 會執行下一步。

### **工作流程中的 AI Agents**

* AI agents 會分別解決小任務。
* 使用者訪問代理會提供 Jon 權限。
* 再次確認後，票據會被關閉。

### **知識工作的定義**

* 知識工作包括許多不同的任務，如：
	+ 對談
	+ 時間表和協調
	+ 道德黑客
	+ 語言和本地化

### **AI Agents 的影響**

* AI agents 可能會對知識工作產生重大影響。
* 需要使用工具來評估這個影響。

**技術變革與工作改變**
==========================

### **O*NET 資料庫**

*   O*NET 是美國勞工統計局的資料庫，收錄了美國經濟中的所有職業。
*   每個職業都有詳細的工作描述、任務清單和技能要求。

### **AI 代理的影響評估**

*   可以使用 O*NET 資料庫來評估 AI 代理對特定任務的影響。
*   這種方法可以幫助決定者和公司制定再培訓計劃，讓員工適應技術變革。

### **技術採用曲線**

*   有些人已經思考過這個問題，並且有相關研究報告。
*   McKinsey 的一份報告提供了對 OECD 國家的預期採用曲線和最壞情況採用曲線的分析。

### **評估方法**

*   **頂部下來**：使用 O*NET 資料庫，嘗試讓 GPT guesses 每個任務的自動化程度。
*   **底部上來**：使用 WorkArena 這個基準來追蹤實際的自動化率。

### **挑戰和限制**

*   這兩種方法都有其局限性，頂部下來的方法可能會模糊，而底部上來的方法可能是不完整。
*   但是，這兩種方法可以幫助我們對技術變革的影響進行三角測量。

**人機協作**
================

### 人機協作的挑戰與機會

*   **技術成熟度**: 確保我們可以在所有人中導航技術成熟度，從而讓所有人受益。
*   **新型態的人機合作**: 人類和機器正在一起工作，開創新的可能性。

### 分工模式

#### **Centaur模式**

*   **策略分工**: 人類負責高層次任務的規劃
*   **AI系統**: 負責大部分的工作

#### **Cyborg模式**

*   **緊密合作**: 人類和機器在解決任務和完成工作時進行非常 granular 的合作

### 未來展望

*   **使用者體驗與電腦人機互動研究**: 這些領域將對於找出最有效的模式有著重要作用
*   **個性型別、工作類型等因素**: 將會影響最佳模式的選擇

### 結論

*   **資源分享**: 提供了一份時間表，讓大家能夠進一步探索LLM代理和基準點。

### 參考資料

*   **框架與基準點**
    *   **2024年之前的框架**
    *   **2024年的新發現**

*   **網頁代理**
    *   **2017年的minima WoB**
    *   **今年的新發現**

---
## 參考資料
- 原始影片：[CS 194/294-196 (LLM Agents) - Lecture 7, Nicolas Chapados and Alexandre Drouin](https://youtube.com/watch?v=-yf-e-9FvOc)
