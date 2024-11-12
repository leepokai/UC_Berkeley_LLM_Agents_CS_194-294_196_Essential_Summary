# CS 194/294-196 (LLM Agents) - Lecture 3, Chi Wang and Jerry Liu

## 課程筆記

**CHI WANG 的演講筆記**
==========================

### 前言
-----------------

* 時間：00:00
* 主題：未來 AI 應用與 AutoGen framework

### 未來 AI 應用
------------------

#### 1. 未來 AI 應用的特點
-------------------------

* **_Generative AI_** 的能力越來越強大
* 能夠生成更好的文本和圖像內容
* 比過去的技術要好得多

#### 2. 未來 AI 應用之路
-----------------------------

* **_Agentic AI_** 的概念：能夠執行複雜任務並幫助人類
* 能夠與人類互動並完成更高級別的任務

### AutoGen framework
---------------------

#### 1. AutoGen framework 的目的
------------------------------

* Empower 每個開發者都能夠建構未來 AI 應用

#### 2. AutoGen framework 的核心問題
--------------------------------------

* **_What are the future AI applications like?_**
* **_How do we empower every developer to build them?_**

### 未來 AI 應用的方向
-------------------------

#### 1. Agentic AI 的概念
-----------------------------

* 能夠執行複雜任務並幫助人類

#### 2. Agentic AI 的應用範圍
----------------------------------

* **_Personal assistants_**
* **_Autonomous bots_**
* **_Gaming agents_**

### 結論
----------

* 未來 AI 應用的方向是 Agentic AI
* AutoGen framework 的目的是 Empower 每個開發者都能夠建構未來 AI 應用

**Agentic AI**
================

### 什麼是 Agentic AI？

*   **自動化**: Agentic AI 可以自動化一些網頁瀏覽和網頁自動化任務，以及軟體代理
*   **軟體代理**: Agentic AI 也可以建立軟體從頭開始

### 示範例子

#### 建立一個網站

*   **模型提取**: Agentic AI 可以從 Hugging Face 提取模型並下載
*   **自動化**: Agentic AI 會根據要求進行分析、尋找資訊和安裝必要的依賴項
*   **多代理框架**: Agentic AI 使用多代理框架來完成任務，包括不同角色和多步驟

#### 自動建站

*   **文件創建**: Agentic AI 會根據需求創建不同的檔案
*   **語言模型**: Agentic AI 使用語言模型進行溝通
*   **代理溝通**: Agentic AI 的代理之間可以進行溝通和協調

#### 自動修正錯誤

*   **錯誤偵測**: Agentic AI 可以偵測到錯誤並自動修正
*   **自我修復**: Agentic AI 有自我修復的能力，能夠在遇到錯誤時進行修正

### 結論

*   **自然界面**: Agentic AI 可以使用更自然的界面與人類溝通
*   **自動化**: Agentic AI 可以自動化一些任務和程序
*   **自我修復**: Agentic AI 有自我修復的能力，能夠在遇到錯誤時進行修正

**Agentic AI 的優點**
=====================

### 一、增強的能力和效率

*   **[06:55]** 給予代理人更多的能力，讓他們能夠完成更複雜的任務，並且需要最少的人類監督。
*   **[07:04]** 這對於自動化有著無窮的價值。

### 二、軟體架構

*   **[07:10]** Agentic AI 可以用作一個新的軟體架構，讓我們能夠建造更複雜的系統。
*   **[07:23]** 這種架構允許多個代理人協同工作，並且完成更多任務。

### 三、實例：供應鏈最佳化

*   **[07:36]** 供應鏈最佳化是一個複雜的問題，需要理解使用者的資料限制和最佳化工具。
*   **[08:14]** AutoGen 可以用來建造代理人，解決這個問題。

### 四、代理人的角色

*   **[08:22]** Commander：接收使用者問題並且啟動其他代理人。
*   **[08:45]** Writer：使用大型語言模型，理解問題並且提出程式碼。
*   **[08:15]** Safeguard：檢查程式碼的安全性。

### 五、結合多個代理人

*   **[08:43]** Commander 和 Writer 的對話：啟動新的對話，並且傳遞程式碼給 Commander。
*   **[09:14]** Commander 和 Safeguard 的對話：檢查程式碼的安全性。

### 六、執行結果

*   **[09:28]** Commander 執行程式碼並且取得結果。

**Agentic Programming**
=======================

### 什麼是 Agentic Programming?

*   **多代理程式設計**: 使用多個代理程式來完成複雜任務。
*   **流程自動化**: 自動化流程和交互模式。

### 流程概述

#### 步驟一：建立代理程式

*   創建多個代理程式（例如，作者、保險箱、指揮官和使用者）。
*   定義代理程式之間的交互模式。

#### 步驟二：定義交互模式

*   記錄兩個嵌套對話給指揮官。
*   為每個嵌套對話定義參與者、發送者和接收者，以及對話摘要方法。

#### 步驟三：定義行為模式

*   定義代理程式的行為模式。

#### 步驟四：啟動聊天

*   啟動使用者代理程式到指揮官代理程式的聊天。
*   發送初始任務需求。
*   其他步驟將自動執行。

### Agentic Programming 的好處

1.  **複雜任務的完成**: 使用多個代理程式來完成複雜任務。
2.  **回應品質的提高**: 多代理程式之間的交互可以改善回應品質。

**Agentic Programming**
=======================

### **分解複雜任務**

*   **分解任務**:將複雜任務分解為更小的任務
*   **多個代理人**:使用多個代理人來完成每個步驟，從而提高質量

### **代理人的設計**

*   **非依賴語言模型**:代理人不需要基於語言模型
*   **特殊用途代理人**:代理人可以根據特定需求進行設計，例如驗證或基於外部知識的驗證

### **實驗結果**

*   **多代理人設定**:將任務分解為兩個代理人，與單一代理人的比較
*   **GPT4 和 GPT3.5 的表現**:多代理人設定比單一代理人設定更好，尤其是在回顧率方面

### **程式設計的益處**

*   **模組化設計**:程式設計時使用模組化設計，可以更容易地理解、維護和擴展系統
*   **自然人參與**:使用模組化設計可以讓自然人輕鬆地加入系統，並與其他代理人進行自然的對話

### **未來發展**

*   **快速創新實驗**:使用多代理人程式設計，可以快速創造新的應用和實驗
*   **挑戰**:設計一個能夠滿足所有需求的框架是困難的，需要考慮許多因素

**Agentic Abstraction**
=======================

### 一. 定義和目的

* **Agentic Abstraction**: 將不同類型的實體（如人、工具或語言模型）統一為一個概念，方便思考和推理。
* 目的是建立一個共同的 AI 系統。

### 二. 關鍵優點

* 利用多代理協調來建造複雜應用
* 方便思考和推理不同類型的實體

### 三. 需要考慮的因素

#### 1. 靜態 vs 動態工作流程

* 開發者可能需要一個靜態的工作流程，以便於追蹤每一步驟
* 或者，開發者可能需要一個動態的工作流程，以便於應對各種情況

#### 2. 自主 vs 控制

* 開發者可能需要給予代理更多自主權，以便於創造更動態的工作流程
* 或者，開發者可能需要控制代理以便於確保精確性

#### 3. 自然語言 vs 程式語言

* 開發者可能需要使用自然語言來指示代理執行任務
* 或者，開發者可能需要使用程式語言來控制代理

### 四. 其他考慮因素

* 分享或隔離代理之間的上下文
* 建立代理之間的合作或競爭關係
* 中央化 vs 分散化
* 自動化 vs 干預

**Agentic AI Frameworks**
==========================

### Introduction

* Agentic AI frameworks are designed to accommodate various design patterns.
* The goal is to have a single framework that can consider all different factors.

### Key Concepts

* **Conversation**: A way of making progress in learning and proving theorems.
* **Multiagent Conversation**: A central mechanism for agentic AI frameworks.
* **Agentic AI Frameworks**: Examples include AutoGen, LlamaIndex, LangChain-based frameworks (LangGraph, CrewAI).

### Agentic AI Frameworks

#### 1. AutoGen
* A programming framework for agentic AI.
* Initially divided from FLAML (automated machine learning and hyperparameter tuning).
* Spun off as a standalone repo with open governance structure.

#### 2. LlamaIndex
* Mentioned but not explained in detail.

#### 3. LangChain-based Frameworks
* Examples include:
	+ **LangGraph**: Focuses on graph-based control flows.
	+ **CrewAI**: Focuses on high-level static agent-task workflows.

### Conclusion

* Agentic AI frameworks have the potential to accommodate various design patterns.
* AutoGen is a notable example of such a framework.

**AutoGen**
================

### 介紹

*   AutoGen 是一個 [21:32] framework with the capability of code execution.
*   在 August, 我們發布了第一版研究論文。
*   在 October, 我們將 repo 移動到 standalone GitHub repo。
*   這得到大量的認可。

### 重要概念

*   **Conversable Agent**
    *   可以抽象不同的實體
    *   可以使用語言模型、工具或人工智慧作為後端
    *   可以混合多種實體
*   **Conversation Program**
    *   可以建立包含其他代理的代理
    *   可以進行內部對話並將其包裝成一個接口

### 使用案例

*   **Sequential Chats**
    *   允許形成進階推理，如反射
    *   例如，可以構建一個作者和一個評論者來改善博客文章的質量
*   **Nested Chat**
    *   可以使用多種推理技巧
    *   例如，使用嵌套對話而不是單一語言模型進行評論

### 其他功能

*   **Group Chat**
    *   允許多個代理進行對話
*   **AI Agentic Design Patterns**
    *   提供了豐富的功能和設計模式

**Nested Chat**
================

### Concept

*   **Sequential Chats**: Construct sequential chats that contain multiple steps of chats.
*   **Reviewer Chain**: Send a message to the SEO reviewer, then to a legal reviewer, ethics reviewer, and so on. Finally, have a meta reviewer summarize all comments and give the final comment.

### Nested Chat Architecture

*   **Single Writer Interface**: From the writer's point of view, it's still talking to a single writer, a single critic agent.
*   **Multiple Agents Underneath**: But underneath, the critic agent uses multiple other agents.

### Example: Building a Game of Conversational Chess

*   **Problem**: Two language model agents playing chess directly often make mistakes and form random moves on the board.
*   **Solution**:
    *   Add a third agent called the chess board. This agent is a tool-based agent that uses Python tools to manage the chess board and provide tools for other language model agents.
    *   The language model agents can only make legal moves, and otherwise, they need to iteratively refine their moves until the moves are legal.

### Nested Chat in Complex Workflows

*   **Group Chat**: In group chat, users only need to define the agents of different roles and then put them in a group chat. The agents automatically decide which agent to speak next depending on the current progress of the task.
*   **Group Chat Manager**: There will be a group chat manager that monitors the progress and makes the selection of speakers.
*   **Constraints or Finite-State Machine Translation Logic**: You can add more constraints or finite-state machine translation logic about what others should follow.

**Autonomous Conversation Patterns**
=====================================

### Introduction

*   **Autonomously**: Can add constraints to ensure selection within scope
*   **Transition Logic**: Use natural language or programming language to specify transitions
*   **Conversation Patterns**: Enable various applications and conversations

### Examples and Domains

#### Notebook Demos

*   Search for specific topics, e.g., integrating AutoGen with LlamaIndex
*   Explore notebook examples on the website, tagged for easy searching

#### Complex Tasks

*   Build complex tasks using simple conversation patterns as building blocks
*   Developers have created various complex tasks using these patterns

### Categories of Domains

*   **Software Development**: Top category, including agent platforms and consulting
*   **Research**: Data processing, web browsing tasks, finance, health education, and blockchain
*   **Science and Engineering Domain**:
    *   Professor Markus Buehler's work on protein design and material design using AutoGen
    *   SciAgents: A team of agents that simulate scientific or engineering teams
        +   Reason about scientific domains using knowledge graphs
        +   Make connections, conduct experiments, and verify hypotheses

### Future Potential

*   Accelerate science discovery with AI-designed medicine, architectures, alloys, and materials

**AutoGen**
================

### 介紹

*   **Agent-E**: 由 Emergence AI 開發的代理程式，使用 AutoGen 建立階層代理團隊，執行複雜任務，如自動預約機票或填寫醫療診所表格。
*   **WebVoyager**: 這個基準測試已經達到最佳性能，但仍有改進空間。

### 基本功能

*   **HTML DOM 檢視**: 能夠深入理解 HTML 內容，不使用多模態模型。
*   **代理程式結合**: 結合代理程式和工作流程，可能提高成功率。

### 企業應用

*   **建設公司**: 使用 AutoGen 幫助非專業人員完成建造工程項目。
*   **MemGPT**: 由伯克利學生創建的 MemGPT 整合了 AutoGen 的功能。

### 進展與改進

*   **評估工具**: 建立代理程式基礎的評估工具，幫助開發者了解應用程式和代理程式的效率。
*   **學習、教導及最佳化**: 提供反饋給代理程式，以便改進其表現。

### 結論

*   AutoGen 已經取得了顯著的進展，企業對其產生了濃厚的興趣，並且有許多貢獻者和使用者從全球各地加入。

**AutoGen**
================

### **中心思想**

*   AutoGen 的核心是改進程式介面，以便讓使用者更容易建立各種代理應用程式。
*   AutoBuild 是一個研究計畫，旨在解決多代理工作流的問題。

### **AutoBuild**

#### **功能**

*   使用者提供任務描述
*   系統會自動建議不同角色代理
*   可以將代理組合在一起，以解決任務

#### **進階功能**

*   可以回顧已建立的代理團隊，以解決新任務
*   可以延伸為適應性代理團隊

### **Adaptive Build**

#### **概念**

*   分解複雜任務成小步驟
*   對每個步驟建議特定代理團隊

#### **實現**

*   可以選擇從已有代理庫中取用或創建新代理
*   逐步檢查並動態選擇代理

### **結果**

*   在數個基準測試中，AutoBuild 的表現優於類似的技術

### **未來工作**

*   設計最佳多代理工作流程
*   考慮多個因素，如品質、成本、延遲和人力投入
*   改進代理能力
*   保證可擴展性
*   提供安全指導

**GitHub Organization**
=======================

### Introduction

* Jerry Liu: Hey, everyone.
* That was a great talk by Chi from AutoGen.

### Building a Multimodal Knowledge Assistant

* **RAG (Retrieval-Augmented Generation)**: 
	+ A specific use case around building a multimodal knowledge assistant.
	+ Focused on principles around RAG and how to extend it.
* **LlamaIndex**: 
	+ A company that helps developers build context-augmented LLM applications from prototype to production.
	+ An open-source toolkit for building agents over data, different types of LLM applications.

### Document Parsing and Data Indexing

* **Document parsing or data parsing**:
	+ A crucial piece in any sort of context-augmented pipeline.
* **RAG components**:
	+ Retrieval from a database to return text chunks.
	+ Embedding the chunk context into a vector database.

### Context-Augmented Pipeline

* **Use cases**: 
	+ Companies with large amounts of data (e.g., PDFs, PowerPoint presentations, Excel files).
	+ Building knowledge assistants for these use cases.

**基本RAG pipeline**
=====================

### 定義

*   **基本RAG**:使用標準文檔解析器將未結構化數據載入，然後將其切割成小塊（每千個令牌），並將每個塊插入嵌入模型中，如OpenAI嵌入模型。
*   **基本RAG pipeline**：整個管道，負責回答基本問題。

### 限制

1.  **數據處理層**:基本RAG的數據處理層相對原始。
2.  **塊切割**:基本RAG不考慮資料內各元素之間的關係。
3.  **使用LLM**:基本RAG僅用於合成，而非推理或計畫。
4.  **一次性執行**:標準RAG管道通常是一次性的，無法個人化。

### 進階應用

*   **進階RAG pipeline**：利用LLM的能力進行更複雜的推理和計畫。
*   **使用模型能力**：盡量發揮最新模型（如01、3.5）的潛力，例如摘要、生成等功能。

**Multimodal Knowledge Assistant**
=====================================

### 一. 問題描述

*   **問題**: 如何建立一個可以回答複雜問題、過多資料的知識助手？
*   **現狀**: RAG ( Retrieve-Augment-Generate ) pipeline 有局限性，無法解答大部分問題。

### 二. 解決方案

#### 1. **Multimodal Retrieval Pipeline**

*   **目的**: 建立一個高質量的多模態檢索管道。
*   **內容**: 能夠處理文本、圖像等不同類型的資料。

#### 2. **Agentic Reasoning**

*   **目的**: 透過工具使用和反思，進行有意義的推理。
*   **內容**: 將 Chain of Thought 等方法應用於問題解答中。

#### 3. **Deployment**

*   **目的**: 部署知識助手並使其可行。
*   **內容**: 規劃和實現知識助手的運作。

### 三. 結論

建立一個能夠回答複雜問題、過多資料的知識助手需要多模態檢索管道、工具使用和反思等多個方面的考慮。

**RAG Pipelines**
================

### 重要概念

*   **ETL**: Extract, Transform, Load
*   **LLM**: Large Language Model
*   **RAG**: Retrieval-Augmented Generator
*   **Data Processing Pipeline**: The process of preparing and processing data for use in a model or application.

### RAG Pipelines 的重要性

*   **Good Data Quality**: A necessary component for any production LLM app.
*   **ETL Layer**: Consists of parsing, chunking, indexing, and putting data into the LLM prompt window.

### 資料處理的挑戰

*   **Complex Documents**: Embedded tables, charts, images, irregular layouts, headers, and footers.
*   **Off-the-shelf Components**: May end up in a broken format when applied to complex documents.
*   **LLM Hallucination**: Users may ask different types of questions over the data, which can lead to incorrect answers.

### 資料處理的步驟

1.  **Parsing**: Structure complex data for any downstream use case.
2.  **Chunking**: Break down large documents into smaller chunks.
3.  **Indexing**: Put data into a format that can be used by the LLM.
4.  **Putting Data into LLM Prompt Window**: Prepare data for use in the LLM.

### 資料處理的挑戰

*   **Bad PDF Parser**: Can lead to incorrect text extraction and hallucination of answers.
*   **Irregular Layouts**: Can make it difficult to parse and chunk documents correctly.

**PDF 解析器**
================

### **概述**

*   **Gen AI-powered PDF parser**: 能夠解析和提取 PDF 文件中的信息。
*   **使用者數量**: 已經有 30,000 多名使用者。

### **功能**

*   **免費試用**: 每天可以獲得 1,000 個信用或頁面。
*   **適用於不同大小的公司**: 由小型企業到大型企業都可以使用。

### **資料結構**

*   **重要概念**：《**PDF 解析器**》、《**資料結構**》、《**向量數據庫**》

#### **資料結構**

##### **提取和解析**

*   **提取和解析 PDF 文件**: 能夠將 PDF 文件中的信息提取出來並進行解析。
*   **提取出不同類型的資料**: 例如投資者簡報、財務報告、Excel 表格等。

#### **向量數據庫**

##### **使用向量數據庫**

*   **使用 Pinecone 或其他向量數據庫**: 能夠對提取出的資料進行索引和存儲。
*   **提取出元資料**: 例如表格的摘要、圖片的描述等。

#### **模型**

##### **多模態模型**

*   **使用多模態模型**: 能夠處理文本和圖像等不同類型的資料。
*   **例如 GPT4.0、Claude 3.5 Sonnet 等模型**: 都可以處理文本和圖像。

### **結論**

*   **PDF 解析器**：是一種能夠解析和提取 PDF 文件中的信息的工具。
*   **資料結構**：是指對於提取出的資料進行索引和存儲的過程。
*   **向量數據庫**：是一種能夠對大量數據進行快速查找和存儲的工具。

**Multimodal RAG Pipeline**
==========================

### **基本概念**

*   **Text Embedding Models**: 用於代表元素本身的模型。
*   **Multimodal RAG Pipeline**: 可以處理任何文檔，並將其轉換為可索引的文本和圖像 chunk。

### **建立 Multimodal RAG Pipeline**

1.  **使用 Text Embedding Models**: 將文本轉換為可索引的 chunk。
2.  **使用 Image Chunk Indexing**: 使用 CLIP embeddings 或模型提取出文本代表並連接到圖像 chunk。
3.  **返回文本和圖像 chunk**: 在檢索過程中，返回兩者，並將其餵給多模態模型。

### **代理機制**

*   **代理設定**: 設定代理機制以便於回答複雜問題。
*   **工具使用**: 使用代理機制來進行工具操作，如生成 PowerPoint 或 PDF。

### **產生完整單位的輸出**

*   **報告生成**: 例如 Claude，可以根據需求生成完整的文檔，並可直接複製和粘貼。
*   **代碼生成**: 可以根據需求生成代碼。
*   **其他功能**: 其他功能如報告、代碼等。

### **企業應用**

*   **知識工作者**: 知識工作者可以使用代理機制來進行報告生成、代碼生成等功能。
*   **顧問**: 顧問也可以使用代理機制來進行報告生成、代碼生成等功能。

**Agentic Reasoning**
=====================

### 什麼是 Agentic Reasoning?

*   **Agentic reasoning**: 是一個在輸入上進行推理的過程。
*   這是一個多模態的RAG管線。

### Agentic RAG 的問題

*   **標準 RAG pipeline**：對於簡單的問題（如點擊式問答）有效，但對於複雜的任務（如總結、比較或高級任務）無法提供良好的結果。
*   **原因**: 由於固定數量的 chunk 被取出，而不是使用 LLM 分析問題。

### Agentic Applications

*   **多種 agentic 應用**：可以建構不同的應用程式，例如：
    *   **ReAct loop**：一個常見的 agent 架構，使用 chain of thought 和 tool use。
    *   **LLMCompiler**：一個 paper，提供了一個更進階的預先規劃功能。

### Agentic Architectures

*   **簡單到進階的 agent 組成部分**：
    *   **ReAct loop**：一個基於 chain of thought 和 tool use 的架構。
    *   **LLMCompiler**：一個提供預先規劃功能的架構。
*   **一般化的 agent 架構**：
    *   **使用工具**：可以插入任何工具，試圖解決任務。

### Agentic Components

*   **簡單到進階的 agent 組成部分**：
    *   **ReAct loop**：一個基於 chain of thought 和 tool use 的架構。
    *   **LLMCompiler**：一個提供預先規劃功能的架構。
*   **一般化的 agent 架構**：
    *   **使用工具**：可以插入任何工具，試圖解決任務。

### Agentic Use Cases

*   **特定的用例**：有些人嘗試解決特定的問題，以建立信任。
*   **更進階的預先規劃功能**：有些人嘗試使用 LLMCompiler 等架構來解決複雜的任務。

**Agentic RAG**
================

### 定義

* Agentic RAG: 一個代理層級在RAG之上的概念
* 代理層級可以決定如何處理查詢和什麼工具要使用來回應

### 特點

* 可以建構更個人化的QA系統
* 能夠處理更複雜的問題

### 流程控制

#### 受限流程

* 有一個明確的任務
* 使用簡單的路由器提示
* 路由器提示選擇下游工具
* 下游工具回應後，使用反射層驗證正確性並生成回應

#### 更一般化代理架構

* 不需要硬編碼流程控制
* 可以使用ReAct、LLM Compiler或Tree of Thought等工具
* 代理可以決定如何處理查詢和什麼工具要使用來回應

**Agentic Architectures**
=========================

### 限制和風險

*   使用過多工具可能會導致無窮迴圈或高昂成本。
*   Marginal token costs 很高。

### 建議

*   對於使用 ReAct 或類似技術的用戶，建議使用四到五個工具，並限制在十個以下。

### LlamaIndex 核心功能

*   帮助用戶建立工作流程。
*   提供核心能力幫助用戶構建工作流程。

### 工作流程定義

*   **_工作流程:_** 基本上是所有使用零件的程式，包括 LLM 呼叫。
*   可以視為一種事件驅動的系統，每一步驟都可以收到訊息，並傳遞給下一個步驟。

### 低層級orchestration

*   提供了一個基礎來幫助用戶將程式轉換成 Python 服務。
*   可以在生產環境中部署工作流程。

### 使用案例

*   報告生成：使用大量資料產生報告的需求是許多公司共同面臨的問題。
*   基於這個需求，LlamaIndex 提供了核心能力幫助用戶建立工作流程。

**Architecture**
================

### Multiagent System

*   **Researcher**: Retrieves relevant chunks and documents from a database.
*   **Writer**: Uses data cache to generate an LLM call that produces a full output.

### Architecture Components

#### Researcher

*   Retrieves relevant information from a database.
*   Stores the retrieved information in a data cache.

#### Writer

*   Uses the data cache to make an LLM call.
*   Generates an interleaving sequence of text, image blocks, tables, and more.

### Example Use Cases

*   **Report Generation**: Generate a report based on the retrieved information.
*   **Slide Deck Generation**: Generate an entire slide deck instead of just a report.
*   **Customer Support**: Automate customer support by baking decision flows into agents to increase deflection rates and improve user experience.

### Running Agents in Production

*   Start building components in a Jupyter Notebook for prototyping.
*   Leverage existing production infrastructure components to achieve a complex multiagent architecture.
*   Encapsulate agent behavior behind an API interface and standardize communication through a core mastering layer.

**多智能網路**
================

### 概念
#### **_Agentic Workflows_**

*   模型每個代理工作流程如服務 API
*   支援本地執行和部署在 Kubernetes 等環境中
*   代理之間的溝通透過中央訊息佇列進行

### 人機互動
#### **_Human-in-the-Loop_**

*   代理可以要求人類提供輸入
*   人類可回應代理的請求
*   代理會根據人類的回應繼續執行

### 案例
#### **_Devon Demo_**

*   Devon 是一個多模態知識助手
*   可以生成程式碼和回答問題
*   人機互動是 Devon 的核心功能

### 未來展望
#### **_Production-Grade Multimodal Knowledge Assistant_**

*   目標是建立一套能夠在生產環境中運行的多模態知識助手
*   這將需要整合多種代理和人機互動技術

---
## 參考資料
- 原始影片：[CS 194/294-196 (LLM Agents) - Lecture 3, Chi Wang and Jerry Liu](https://youtube.com/watch?v=OOdtmCMSOo4)
