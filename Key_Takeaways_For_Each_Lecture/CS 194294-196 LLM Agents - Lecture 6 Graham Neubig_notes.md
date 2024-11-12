# CS 194/294-196 (LLM Agents) - Lecture 6, Graham Neubig

## 課程筆記

**軟件開發代理人**
================

### Graham Neubig 的介紹

*   CMU 教授
*   All Hand AI 首席科學家
*   Open Hands (以前稱為 Open Devon) 維護者
*   軟體開發者

### 代理人的重要性

*   Marc Andreessen 的論文《為什麼軟件正在吞噬世界》(2011)
	+   多個行業正在被軟件取代
	+   未來十年將有更多行業受到軟件的影響
*   軟件開發代理人能夠幫助大家快速創建軟件

### 研究和實踐

*   如果我們給每個人能力快速創建軟件，什麼樣的事情會發生？
	+   對於計算機科學家來說，這將是一個巨大的改變
*   軟件開發代理人能夠幫助大家達成目標

### 結論

*   軟件開發代理人的重要性在日益增強
*   這將對我們的生活和科學進步產生重大影響

**軟件開發模型**
================

### 時間分配

*   人員平均每天花費的時間在撰寫新代碼方面只佔15%。
    *   這是根據2019年的微軟研究結果。

### 軟件開發工作內容

*   **程式設計**
    *   15%
*   **Bug修正**
    *   10%
*   **測試**
    *   8%
*   **文件撰寫**
    *   4%
*   **評論**
    *   3%
*   **溝通**
    *   36%
*   **其他事項**
    *   17%

### 自動化類型

#### 軟件開發自動化

*   **零級自動化**
    *   手工撰寫代碼
*   **一級自動化**
    *   智慧型完成敘述
    *   例如Copilot或Cursor
*   **二級自動化**
    *   自動完成程式碼重構
    *   例如Copilot或Cursor聊天機器人
*   **三級自動化**
    *   對特定任務進行自動化
*   **四級自動化**
    *   全面自主的軟件開發

### 自動完成程式碼

*   **Copilot**
    *   智慧型完成敘述
    *   可以填寫程式碼
*   **Cursor**
    *   智慧型完成敘述
    *   可以填寫程式碼

**Autonomous Issue Resolution**
=====================================

### 什麼是 Autonomous Issue Resolution?

*   自動解決 GitHub 問題的能力
*   使用 AI 和機器學習來自動完成程式碼修改和測試

### 例子

#### 解決 GitHub 問題

*   下載 GitHub repo
*   建立新的測試
*   安裝依賴項
*   執行測試
*   提交更改並推送到 GitHub

#### 自動解決問題的流程

1.  標記問題為 "Fix Me"
2.  AI 代理人執行動作
3.  如果成功，AI 代理人會發出拉取請求
4.  人類可以檢視和確認更改

### GitHub Copilot 的研究結果

*   研究中有 95 名開發者參與
*   使用 GitHub Copilot 的開發者完成任務的比例比不使用 Copilot 的開發者高 8%
*   使用 Copilot 的開發者完成任務的速度比不使用 Copilot 的開發者快 56%

### 結論

*   自動解決問題的能力可以大幅度提高開發者的效率
*   GitHub Copilot 等工具可以幫助開發者快速完成程式碼修改和測試

**軟件開發環境**
================

### 軟件開發挑戰

*   **定義環境**: 如何讓程式碼代理（coding agents）能夠在一個可測試的環境中運作？
*   **設計觀察和行動空間**: 如何讓程式碼代理能夠與環境互動？

### 軟件開發代理挑戰

#### 產生程式碼

*   **語言模型**: 使用哪些程式語言模型來生成程式碼？
*   **建構模型**: 如何建立這些程式語言模型？

#### 編輯程式碼

*   **檔案定位化**: 如何識別程式碼中的哪些部分需要編輯？

#### 計劃和錯誤恢復

*   **計畫**: 如何讓程式碼代理能夠制定計畫？
*   **錯誤恢復**: 如何讓程式碼代理能夠從錯誤中恢復？

#### 安全性

*   **安全環境**: 如何確保程式碼代理能夠在一個安全的環境中運作？

### 軟件開發環境

#### 類型

*   **源代管系統**: 如何讓程式碼代理能夠與 GitHub、GitLab 等系統互動？
*   **任務管理軟體**: 如何讓程式碼代理能夠與 Jira、Linear 等系統互動？
*   **辦公軟體**: 如何讓程式碼代理能夠與 Google Docs、Microsoft Office 等系統互動？
*   **溝通工具**: 如何讓程式碼代理能夠與 Gmail、Slack 等系統互動？

#### 其他環境

*   **伺服器**: 如何讓程式碼代理能夠與伺服器互動？
*   **雲基礎設施**: 如何讓程式碼代理能夠與雲基礎設施互動？

**軟件開發測試**
================

### **簡介**

*   目前有許多程式碼生成相關的測試可供使用。
*   這些測試大部分都是基於程式碼生成。

### **程式碼生成測試**

#### **簡單程式碼生成**

*   **定義**: 測試程式語言模型從規格到程式碼的能力。
*   **範例**:
    *   HumanEval
    *   MBPP

#### **程式碼生成基礎**

*   **定義**: 測試程式語言模型對程式碼生成的基本能力。

### **程式碼生成基準**

#### **CoNaLa**

*   **定義**: 基於Stack Overflow資料進行程式碼生成基準測試。
*   **特點**:
    *   包含了較廣泛的程式庫，例如Pandas、NumPy等。

### **程式碼生成基準的重要性**

*   **程式碼生成基準**: 測試程式語言模型對程式碼生成的能力。
*   **程式碼生成基準的類型**:
    *   基於程式碼生成
    *   基於執行結果評估

### **程式碼生成基準的應用**

*   **程式碼生成基準**: 測試程式語言模型對程式碼生成的能力。
*   **程式碼生成基準的類型**:
    *   基於程式碼生成
    *   基於執行結果評估

**Python Ecosystem**
=====================

### 重要概念

*   **Data Science Notebooks**: 使用資料科學筆記本來進行增量式實現和評估程式碼。
*   **SWEBench**: 一個相對較新的資料集，基於 GitHub 問題和代碼庫的爬蟲結果。

### 重要概念

#### Data Science Notebooks
-----------------------------

*   使用資料科學筆記本來進行增量式實現和評估程式碼。
*   可以在筆記本中生成下一個細胞，基於已有的上下文。

#### SWEBench
----------------

*   一個相對較新的資料集，基於 GitHub 問題和代碼庫的爬蟲結果。
*   可用來評估程式碼修改和測試的能力。

### 重要概念

#### Pass@K
-------------

*   測量程式碼生成成功率的一個指標。
*   如果生成 K 個範例中至少有一個能通過單元測試，則視為成功。

### 限制與挑戰
-------------------

*   SWEBench 的資料集可能存在偏差和漏洞。
*   測量程式碼生成成功率的變異性可能會很高。

**Code Generation Methods**
==========================

### 1. **統計方法**

*   使用統計方法生成 `n` 個代碼，並根據統計數據計算出在 `K` 個代碼中的準確率。
*   這是最常見的方法，但需要單元測試，因此只能應用於有單元測試的情況下。

### 2. **語義重疊方法**

*   基於語義重疊進行代碼生成
*   這種方法會比較生成代碼與程式設計師創建的金標準代碼之間的重疊程度

#### 2.1 **BLEU 方法**

*   使用BLEU方法計算代碼生成的準確率
*   BLEU方法基於n-gram重疊進行計算

#### 2.2 **嵌入法**

*   使用嵌入法進行代碼生成評估
*   嵌入法包括CodeBERTScore等方法

### 3. **資料集泄露問題**

*   資料集泄露是程式設計中的一個嚴重問題
*   這會導致模型過度依賴特定的資料集，從而影響其泛化能力
*   SWEBench Plus是一篇關於此問題的研究論文

#### 3.1 **SWEBench Plus**

*   這篇論文評估了程式設計模型在不同資料集上的表現
*   結果顯示，模型在未見過的資料集上表現不佳

#### 3.2 **ARCADE**

*   ARCADE是一個程式設計模型評估工具
*   這個工具使用實際的人工智慧模型創建的代碼進行評估
*   結果顯示，模型在未見過的資料集上表現不佳

#### 3.3 **LiveCodeBench**

*   LiveCodeBench是一個程式設計模型評估工具
*   這個工具使用實際的人工智慧模型創建的代碼進行評估
*   結果顯示，某些程式設計模型在特定的資料集上表現優異

### 4. **多模態程式設計**

*   多模態程式設計是一種新興的研究方向
*   這種方法會使用多種資訊來進行程式設計

**Design2Code**
================

### Introduction

*   Design2Code是一個由斯坦福大學開發的資料集，用於生成代碼。
*   它通過分析網站設計來產生代碼。

### Features

*   **視覺相似性測試**
    *   生成網站
    *   取得網站截圖
    *   進行高級和低級視覺相似性測試

### 相關概念

#### 代碼代理人

*   代碼代理人必須能夠理解程式庫結構、讀取現有代碼、修改或產生代碼、執行代碼和偵錯。

#### 觀察行動空間

*   代碼代理人的觀察行動空間包括：
    *   檢視程式庫結構
    *   讀取現有代碼
    *   修改或產生代碼
    *   執行代碼和偵錯

#### 代碼代理人範例

*   **CodeAct**
    *   CodeAct是一種方法，它通過寫代碼來與環境互動。
    *   它是用於開放手的代碼模型的代碼平台。

### 相關資料集

*   **SWEBench**
    *   SWEBench是一個多模態版本的資料集，類似於Design2Code。

**CodeAct**
================

### 問題描述

傳統模型會一步一步地執行查詢、轉換等動作，可能需要多次 API 呼叫才能得到最終答案。

### CodeAct 的建議

*   移除單步工具使用的限制
*   讓模型能夠撰寫程式碼
*   可以在少數步驟中完成複雜任務

### 例子

*   使用 `for` 迴圈遍歷所有國家，執行查詢等動作
*   在錯誤時，可以回頭修改程式碼並重新執行

### 相關概念

#### **SWE-Agent**

*   定義特殊工具來高效探索程式庫和編輯代碼
*   可以在少數步驟中完成複雜任務

#### **LM Friendly Commands**

*   對語言模型友好的命令，能夠與電腦、終端機和檔案系統互動
*   可以提供環境反饋

### 例子

*   使用 `show file` 命令觀看程式碼
*   選擇特定行後，可以取得程式碼的窗口

### 結論

CodeAct 的建議可以讓模型在少數步驟中完成複雜任務，提高效率和成功率。

**Code-Based LLMs**
=====================

### 什麼是 Code-Based LLMs?

* **Code-Based LLMs** 是指基於程式碼的語言模型 (LLMs)
* 這類模型能夠理解和生成程式碼
* 能夠幫助開發者解決程式碼相關問題

### Code-Based LLMs 的應用

* **程式碼編輯**: 能夠自動完成程式碼編輯工作
* **程式碼分析**: 能夠分析程式碼並提供意見
* **程式碼生成**: 能夠基於給定的條件生成程式碼

### Code-Based LLMs 的方法

* **SWE-Agent 方式**: 一種程式碼編輯方式
* **OpenHands 方式**: 類似於 CodeAct 和 SWE-Agent 方式的程式碼編輯方式

### Code-Based LLMs 的重要性

* **程式碼理解**: 能夠幫助開發者更好地了解程式碼
* **程式碼生成**: 能夠基於給定的條件生成程式碼
* **程式碼分析**: 能夠分析程式碼並提供意見

**程式語言模型**
================

### 概念介紹

*   **GPT、Claude、Gemini等模型**: 這些是程式語言模型的代表，能夠理解和生成程式碼。
*   **特殊化**: 有些模型更為專業化，針對特定領域或程式語言進行訓練。

### 訓練資料

#### 代碼數據

*   **大量代碼數據**: 這是所有程式語言模型的共同點。
*   **程式碼數據的重要性**: 進一步訓練程式能力和推理能力。
*   **研究結果**: 前人的研究證實，加入程式碼數據能夠改善模型的推理能力。

#### The Stack 2

*   **開放資料集**: 這是已經被用於訓練開放模型的代碼預訓練數據集。
*   **授權考慮**: 進行了授權清潔和其他相關工作，以避免法律問題。

### 代碼語言分布

#### 流行程式語言

*   **Python、PHP、Markdown、JavaScript、Java、C++、C#、C**: 這些是最常見的程式語言。
*   **代表性**: 這些程式語言在開發者中非常受歡迎。

#### 少見程式語言

*   **Docker文件**: 這是一種重要但相對少見的程式語言。
*   **Terraform**: 這是用於部署雲端基礎設施的程式語言，但在這個資料集中並未被代表。

### 未來發展

#### COBOL

*   **舊程式語言**: 這是一種已經過時的程式語言，但仍然存在於銀行等行業的舊系統中。
*   **轉換需求**: 這些舊系統需要被轉換為現代程式語言。

#### 未來發展方向

*   **程式語言模型的進一步特殊化**: 進一步針對特定領域或程式語言進行訓練。

**重要概念**
* **Infilling**: 在編碼生成中填充代碼
* **Code Generation**: 編碼生成
* **Pre-training method**: 預訓練方法
* **Long context extension**: 長文本擴展
* **Positional encodings**: 位移編碼
* **Rope**: 位移編碼的一種
* **Neural tangent kernel-based method**: 神經彎曲核基方法

**項目符號列表**

### 1. Infilling

* 是在編碼生成中填充代碼的過程
* 使用預訓練方法來訓練模型
* 每個嚴肅的編碼模型都會使用此方法

### 2. Code Generation

* 編碼生成是使用模型產生代碼的過程
* 需要使用預訓練方法和長文本擴展
* 每個嚴肅的編碼模型都會使用此方法

### 3. Pre-training method

* 預訓練方法是一種用於訓練模型的方法
* 使用原始文件和遮罩技術來填充代碼
* 可以提高模型對編碼生成的能力

### 4. Long context extension

* 長文本擴展是使用模型延伸長文本的過程
* 需要使用位移編碼和神經彎曲核基方法
* 每個嚴肅的模型都會使用此方法

### 5. Positional encodings

* 位移編碼是一種用於表示位置信息的技術
* 使用 rope 等方法來實現
* 可以提高模型對長文本的能力

### 6. Rope

* rope 是一種位移編碼的一種
* 使用 theta 值來表示位置信息
* 可以提高模型對長文本的能力

### 7. Neural tangent kernel-based method

* 神經彎曲核基方法是一種用於實現神經網路的方法
* 使用 cosine 和 sine 值來表示高頻率和低頻率成分
* 可以提高模型對長文本的能力

**長距離程式設計**
=====================

### 問題與挑戰

*   **程式設計緊張感**: 過長的程式碼距離會導致程式設計緊張感增加。
*   **本地化上下文**: 長距離程式設計需要考慮本地化上下文。

### 解決方案

#### 1. **長距離程式設計延伸**

*   Lu 等人的研究 paper 提供了更多細節的解釋。

#### 2. **程式碼模型與資訊**

*   **程式碼模型**: Copilot 等程式碼模型會取用大量資訊。
*   **可用的資訊**: 可用的資訊包括:
    *   **目前程式碼上下文**
    *   **問題描述**
    *   **程式庫資訊**
    *   **開啟的 IDE tabs**

#### 3. **檔案本地化**

*   **檔案本地化**: 檔案本地化是程式設計中的重要挑戰。
*   **使用者意圖**: 根據使用者的意圖找到正確的檔案。

### 未來發展方向

#### 1. **程式碼模型與資訊**

*   **程式碼模型**: Copilot 等程式碼模型需要進一步的改善。
*   **提示工程**: 提供更多相關資訊以提高程式碼建議的準確性。

#### 2. **檔案本地化**

*   **檔案本地化**: 檔案本地化是程式設計中的重要挑戰。
*   **未來發展方向**: 進一步研究和改善檔案本地化以提高程式碼建議的準確性。

**Rejecting an Action and Providing Feedback**
==============================================

### Problem Statement

*   **Localisation Problem**: An action is rejected, but the system doesn't know about it.
*   **Solution Request**: A third option "confirm action in wait" to provide feedback before proceeding.

### Solution Options

#### 1. Offload to User

*   **Description**: The user is responsible for providing information to the agent.
*   **Limitations**:
    *   Requires a user familiar with agents and their capabilities.
    *   Not applicable to all users, especially those without knowledge of the code base.

#### 2. Prompt Agent with Search Tools

*   **Example**: SWE-Agent provides a search tool for searching repositories.
*   **Description**: The agent is prompted to search for relevant information before proceeding.

### Key Concepts

*   **Embodied Agents**: Agents that interact with their environment, such as robots in a kitchen.
*   **Localisation Problem**: Understanding the environment and retrieving relevant information.

### Related Issues

*   **Understanding Environment**: Embodied agents need to understand their environment before solving problems.
*   **Retrieval Time**: Agents need to have a good system for retrieving relevant information.

**Agent-Based Systems**
=======================

### 搜尋和總結搜尋結果

*   **使用工具**: 可以使用工具來搜尋和總結搜尋結果，提供必要的資訊。
*   **開發人員工具**: 有許多開發人員工具可以幫助這個過程，例如 Ada。

### 建立程式碼庫地圖

*   **建立程式碼庫地圖**: 可以使用工具來建立程式碼庫的地圖，方便搜尋和總結。
*   **Ada 工具**: Ada 是一個開源工具，可以創建樹狀結構的程式碼庫地圖。

### 代理人無法搜索

*   **代理人無法搜索**: 這是一種方法，會對每個問題進行階層式搜尋。
*   **使用代理人**: 使用代理人的過程中，需要提供一個簡單的樹狀結構來代表程式碼庫。

### 取得程式碼

*   **取得程式碼**: 代理人可以根據程式碼庫的地圖，取得所需的程式碼。
*   **程式碼總結**: 代理人可以對程式碼進行總結，以便於理解。

### 本地化功能

*   **本地化功能**: 代理人需要將程式碼本地化到特定的函數中。
*   **顯示程式碼**: 代理人會顯示程式碼給使用者，以便於編輯和修改。

### 取得相似程式碼

*   **取得相似程式碼**: 這是一種方法，會根據程式碼庫的地圖，取得相似的程式碼。
*   **程式碼生成**: 代理人可以根據程式碼進行生成，包括程式碼和文件。

### 文件的重要性

*   **文件的重要性**: 文件對於程式碼的理解非常重要。
*   **直接取文件**: 有時候需要直接取文件來生成程式碼。

**Planning and Error Recovery**
=====================================

### Unsolved Problem: Leverage [45:45] Effectively

*   **[45:45]** is not effectively used in agentless setting yet.
*   People will probably move towards this direction, but there might be new archive papers that have been missed.

### Planning and Error Recovery

#### Solving Coding Tasks

*   Solving coding tasks can be difficult.
*   A plan and tracking progress are essential to solve the tasks effectively.

#### Top Coding Models

*   Many top coding models or agent models have a hardcoded task completion process.
*   Agentless is an example of this, where it mostly goes through a process containing three steps: file localization, function localization, and generating patches.

#### Planning Methods

*   **Agentless** gets good results for its simplicity but is inflexible.
*   Hardcoded methods cannot be modified or extended easily.
*   Multi-agent style methods or methods using LLM-generated plans beforehand are less inflexible.

#### Example: Coder

*   The coder multi-agent system generates a plan based on subagents like reproducer, fault localizer, editor, and verifier.
*   It has a semi-hardcoded structure between agents where a plan is first generated.

**Structured Architecture for Solving GitHub Issues**
===========================================================

### 重要概念

*   **Reproducer Step**: reproducing the issue to verify its existence
*   **Fault Localization Step**: identifying the root cause of the issue
*   **Editor Step**: modifying the code to fix the issue
*   **Verifier Step**: verifying that the modified code fixes the issue
*   **Hard Coded Control Flow**: a predefined sequence of steps to solve issues

### 流程描述

#### reproducer step

1.  reproducer runs the code with the reported issue
2.  if able to reproduce, send to fault localizer; otherwise, send directly to editor

#### fault localization step

1.  identify the root cause of the issue
2.  modify the code accordingly

#### editor step

1.  modify the code based on the identified root cause
2.  verify that the modified code fixes the issue

### 問題和挑戰

*   **Language Model Agents**: often generate plans that are not optimal
*   **Plan Revision**: need to revise plans when underlying assumptions are incorrect
*   **Looping Issues**: models can get stuck in a loop trying to fix an issue

### 解決方案

*   **Kick-Back Mechanism**: allow the agent executing the plan to kick it back to the planner if fails
*   **Plan Revision**: enable the planner to generate a new plan based on feedback from the agent
*   **Fix Outputs Based on Error Messages**: have agents run code, see results, and fix code accordingly

### 未來方向

*   **Inter Code**: an example of fixing outputs based on error messages
*   **GP 4.0**: has issues with attempting to fix an issue, failing, and getting stuck in a loop
*   **Claude**: better at not getting stuck in a loop and trying different approaches

**Error Recovery**
================

*   **重要概念**: 
    *   **錯誤恢復**
    *   **安全性**

### 1. 錯誤恢復

*   錯誤恢復將成為未來的一個大研究主題。
*   人們正在努力解決這個問題。

### 2. 安全性

*   編碼模型可能會造成傷害。
*   我最擔心的是編碼模型因為意外或誤解而導致的損害。
*   **實例**:
    *   問一個編碼模型將程式碼提交到 GitHub 仓库。
    *   這個模型可能會誤解命令，直接推送程式碼至主分支。

### 3. 安全性措施

*   **沙盒化**: 
    *   限制模型的環境訪問權限。
    *   **範例**:
        *   Open Hands 使用 Docker 環境執行所有動作，隔離於主要系統中。
        *   這樣可以控制模型對檔案和網路訪問的權限。

### 4. 意圖性誤用

*   編碼模型可能會被用於惡意攻擊等活動。
*   我們需要謹慎地設計安全措施以防止這種情況發生。

**安全性與軟件**
================

### 安全性工具的重用

*   **[54:52]** 已經對軟件安全性進行了大量思考，可以重用已知的工具。
*   **Docker** 是一個例子，能夠重用在非代理場景下的工具。

### 權限管理

#### 最小權限原則

*   **[55:24]** 人員應該只擁有必要的權限做其工作。
*   **[55:31]** 服務應該只擁有必要的權限做其工作。

#### GitHub存取令牌

*   **[55:38]** 存取令牌可以具有非常細緻的權限，允許在特定GitHub存儲庫上進行特定的操作。
*   **[56:02]** 可以選擇讓它對所有公共存儲庫有讀取權限，或是只允許訪問自己擁有的存儲庫。

### 代理安全性

#### 最小權限原則的應用

*   **[56:32]** 可以防止代理獲得超出其需要的權限，但仍然提供它所需的權限。
*   **[56:41]** 可以輕易地創建一個完全無用的代理，只需將它放在沙盒中，並不給予任何權限。

### 后續審計

#### 模型后續審計

*   **[57:07]** 可以生成動作，然後根據動作的性質決定是否執行。
*   **[57:38]** 如果動作被視為有害，可以不執行並返回警告訊息。

**Coding Agents**
================

### 介紹

*   **Joint work with Invariant Labs and ETH**
*   **結論**: Copilots 是非常有用的, code agents 還在發展中

### 成果

*   **Copilots 的實用性**: 已經證明 Copilots 很有用
*   **Code Agents 的進展**: Code agents 正在發展中

### 未來方向

*   **Agentic Training Methods**
    *   **Training on agent style data**: 這將使我們能夠遵循代理格式, 做更好的規劃, 並從錯誤中恢復
*   **Human in the Loop Methods for Evaluating Agents**
    *   **評估代理的最佳方式**: 還沒有明確的方法來評估代理

### 其他挑戰

*   **Good Code, LLMs, Editing Methods, Localization, Planning and Safety**

### 未來展望

*   **Coding Agents 的發展**: 在未來的一到兩年內, Coding Agents 將能夠幫助我們完成許多日常任務
*   **代理的進步**: 代理將會逐漸改善, 能夠完成需要更多思考和關懷的事項

### 其他資源

*   **Software Toolkit**: 可以下載軟件工具包, 這些工具包能夠幫助我們完成許多任務
*   **Feedback and Collaboration**: 感謝您的反饋和合作

---
## 參考資料
- 原始影片：[CS 194/294-196 (LLM Agents) - Lecture 6, Graham Neubig](https://youtube.com/watch?v=f9L9Fkq-8K4)
