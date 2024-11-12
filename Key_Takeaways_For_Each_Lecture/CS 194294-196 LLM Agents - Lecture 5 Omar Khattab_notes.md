# CS 194/294-196 (LLM Agents) - Lecture 5, Omar Khattab

## 課程筆記

**工作與大量人合作**
========================

### 工作背景

*   **大型語言模型**: 這是與許多人共同工作的例子，超過 200 名貢獻者。
*   **滑片**: 使用許多滑片，包括 Krista 和 Michael 的作品。

### AI 應用

*   **ChatGPT**: 一個非常成功的 AI 應用程式，可以回答使用者的任何問題，並且能夠在實時對話中合成答案。
*   **語言模型的優勢**: 能夠幫助使用者完成任務，例如編寫代碼。

### 限制

*   **語言模型的弱點**: 這些模型容易出錯，而且難以檢測。
*   **ChatGPT 的例子**: 使用 ChatGPT 幫助編寫代碼時，我們需要小心避免錯誤。

### 結論

*   **系統可靠性**: 即使能夠輕鬆地建立令人印象深刻的 AI 應用程式，仍然很難建立可靠的 AI 系統。
*   **系統控制**: 我們需要找到方法來控制和改善這些系統，以避免錯誤並進行進一步的開發。

**Compound AI Systems**
=======================

### 什麼是 Compound AI Systems?

*   **定義**: 模組化系統或模組化程式，使用語言模型在更大的架構中扮演特殊角色。
*   **範例**:
    *   **Retrieval Augmented Systems (RAG)**: 使用語言模型和知識庫來回答問題。

### 優點

#### 透明度
*   可以檢視系統行為的痕跡，了解它如何使用資訊。
*   有助於判斷系統是否正確或錯誤。

#### 效率
*   可以將知識和控制流程分散到知識庫和執行程序中。
*   這樣可以減少語言模型的負擔，提高效率。

**多跳推理或多跳檢索**
========================

### **系統架構**

*   **多跳推理或多跳檢索**：使用 AI 系統進行多步驟的推理或檢索
*   **增強生成**：使用 AI 系統進行增強生成

### **系統控制**

*   **控制度**: 人們可以控制系統的發展，無需等待語言模型的下一次更新
*   **快速迭代**: 可以快速地進行系統的改進和優化

### **系統應用**

*   **長篇報告**：使用 AI 系統生成長篇報告，如文章或維基百科頁面
*   **模組化設計**：使用多個模組來進行系統設計，例如腦storm、生成草圖、修改草圖等

### **優點**

*   **質量控制**: 可以控制系統的質量和效率
*   **快速迭代**: 可以快速地進行系統的改進和優化
*   **推理能力**：可以使用多步驟的推理來取得更好的結果

**Compound AI System**
=======================

### 什麼是 Compound AI System?

*   **定義**: Compound AI system 是一種結合多個 AI 模型的系統，透過這些模型之間的互動來達成更複雜的任務。
*   **範例**: AlphaCodium 是一個 Compound AI system 的例子，它用於生成程式碼。

### Compound AI System 的優點

*   **分解複雜任務**: Compound AI system 可以將複雜任務分解成多個較小的任務，透過這些任務之間的互動來達成最終目標。
*   **提高效率**: 透過 Compound AI system，可以提高程式碼生成等任務的效率。

### Compound AI System 的限制

*   **語言模型的局限性**: Compound AI system 依賴於語言模型，然而這些模型本身有著局限性。
*   **對語言模型的敏感度**: Compound AI system 需要根據特定的任務來調整語言模型，以達成最佳效果。

### 未來發展方向

*   **開發更強大的語言模型**: 透過開發更強大的語言模型，可以提高 Compound AI system 的效率和準確度。
*   **研究如何更好地調整語言模型**: 研究如何更好地調整語言模型，以適應不同任務的需求。

**五個角色**
================

### 角色一：簽名角色
-----------------

*   該角色試圖涵蓋
*   是一個功能，提供這個模組。
*   它基本上就是一個規格，
    *   這裡是你的輸入，
    *   這裡是輸入的含義，
    *   這裡是你想要的轉換，
    *   來給我輸出。

### 角色二：計算角色
-----------------

*   該角色試圖涵蓋
*   試圖透過推理時的策略，
    *   將簽名角色特殊化。
*   你可能告訴模型，
    *   請一步一步地思考，
    *   或告訴模型，
    *   您是一個代理人，
    *   您有這些工具，
    *   您應該叫用這些工具。

### 角色三：對象角色
-----------------

*   該角色試圖涵蓋
*   當你叫用工具時，
    *   我會攔截它。
    *   我會給你回應。

### 角色四：探索角色
-----------------

*   該角色試圖涵蓋
*   生成10個不同的東西，
    *   這些東西都會被用來探索，
    *   使用一些獎勵模型。

### 角色五：對象角色
-----------------

*   該角色試圖涵蓋
*   將所有輸入都格式化好，
    *   將所有輸入都給這個功能或簽名。
*   這也包括了逻辑，
    *   逐步地解析和轉換輸入，
    *   如果輸入不夠正確，則重新嘗試。

### 角色六：目標角色
-----------------

*   該角色試圖涵蓋
*   將所有輸入都格式化好，
    *   這也包括了逻辑，
        +   逐步地解析和轉換輸入，
        +   如果輸入不夠正確，則重新嘗試。
*   這也包括了目標，
    *   你不是只是描述輸入和輸出行為，
    *   你還試圖在提示中包含許多信息，
        +   什麼是可以做的，
        +   什麼是不可以做的，
        +   什麼是你想要最大化的。

### 角色七：敏感角色
-----------------

*   該角色試圖涵蓋
*   這些管道非常複雜。
*   人們會花很大的力氣，
    *   對模型進行試驗和錯誤，
    *   來讓它做正確的事情。

### 角色八：微調角色
-----------------

*   該角色試圖涵蓋
*   這些管道非常複雜。
*   人們會花很大的力氣，
    *   對模型進行試驗和錯誤，
    *   來讓它做正確的事情。

### 角色九：整體角色
-----------------

*   該角色試圖涵蓋
*   這些管道非常複雜。
*   人們會花很大的力氣，
    *   對模型進行試驗和錯誤，
    *   來讓它做正確的事情。

### 角色十：整體角色
-----------------

*   該角色試圖涵蓋
*   這些管道非常複雜。
*   人們會花很大的力氣，
    *   對模型進行試驗和錯誤，
    *   來讓它做正確的事情。

**developer 的問題**
=====================================

### 問題描述

*   **無法重現結果**: 當 pipeline 或 language model 變化時，原有的 prompt 會變得無效。
*   **無法轉移系統**: 原有的系統無法在不同環境下運行。

### 解決方案

#### 使用程式設計的方法

*   **使用模組化的方法**: 將 AI 系統分解為多個可重用的模組。
*   **使用自然語言功能**: 將自然語言功能整合到程式碼中，讓系統能夠學習和改善。

#### 優點

*   **提高可移植性**: 可以在不同環境下運行。
*   **降低成本**: 不需要重寫 prompt 或重新訓練模型。

**DSPy**
================

### 重要概念

*   **Declaratively Self-Improving (DS)**: 一種自我改進的程式設計方法
*   **Language Model Program**: 一個用於語言模型的程式設計方法
*   **Fuzzy Functions**: 模糊函數，指的是可以根據上下文進行解釋和執行的函數

### DSPy 的核心理念

#### 1. 高級抽象層

DSPy 的目標是建立一個高級抽象層，使程式設計師能夠撰寫程式碼而不必關心底層細節。

#### 2. 自我改進

DSPy 的自我改進功能使得程式可以根據使用者的反饋和執行結果進行改進。

### DSPy 的工作流程

1.  **定義語言模型程式**: 定義一個語言模型程式，該程式可以接收自然語言的輸入並產生相應的輸出。
2.  **執行程式**: 執行語言模型程式，該程式會根據輸入進行處理和產生輸出。
3.  **自我改進**: 根據程式的執行結果和使用者的反饋進行自我改進。

### DSPy 的優點

*   **簡單易用**: DSPy 提供了一個高級抽象層，使程式設計師能夠撰寫程式碼而不必關心底層細節。
*   **自我改進**: DSPy 的自我改進功能使得程式可以根據使用者的反饋和執行結果進行改進。

### DSPy 的應用範圍

DSPy 可以應用於各種領域，例如自然語言處理、機器學習等。

**Fact Checking Module**
=======================

### 目標
-----------------

* 建立一個 Fact Checking 模組，能夠評估一系列的聲明是否真實

### 需求
------------

* 清理程式碼中的迴圈、例外和註解
* 運用 Chain of Thoughts 策略來評估程式簽名
* 將一系列的聲明傳入模組，獲得真實性判斷結果

### 模組功能
-------------

* 接受一系列的聲明
* 評估每個聲明的真實性，並返回一個布林值陣列
* 提供一個接口，讓使用者能夠傳入聲明並獲得評估結果

### 關鍵概念
----------------

* **Chain of Thoughts**: 運用一系列的邏輯推理來評估程式簽名
* **Natural Language Types**: 使用自然語言類型來定義程式簽名
* **Optimization Problem**: 建立一個最佳化問題，目的是最大化程式執行時的效率

### 問題難度
-----------------

* 這是一個困難的最佳化問題，不涉及梯度下降法
* 需要建立一個系統來生成和執行程式碼

**系統優化**
================

### 問題點

* 系統可能會呼叫外部工具
* 可能需要運行計算機
* 不清楚如何直接使用梯度來優化系統
* 不能假設每個模塊都有標籤
* 這樣做會破壞迭代開發和模組化的理想

### 具體範例

#### 多跳查詢增強生成管道

* 建立一個多跳查詢增強生成管道
* 每個步驟都需要標籤
* 但我們不能假設每個步驟都有標籤
* 這會使系統優化變得困難

### 問題點

* 我們不知道如何優化這種系統
* 我們無法假設每個模塊都有標籤
* 這會破壞迭代開發和模組化的理想

**Kinnordy Castle**
================

### 重要概念

*   **DSPy**: 
*   **PyTorch**: 
*   **Chain-of-Thought**: 
*   **Signature**: 

### 概要

#### Kinnordy Castle

1.  **Kinnordy Castle** 是一個名為 Kinnordy 的城堡。
2.  城堡有多層樓。

#### Chain-of-Thought

1.  **Chain-of-Thought** 是一種策略，能夠生成搜索查詢和答案。
2.  策略需要輸入上下文和問題。
3.  這些輸入都是字串。

#### Signature

1.  **Signature** 是一個描述模組功能的方法。
2.  它告訴系統該做什麼，而不是如何做。

### 模組結構

#### 初始化方法

1.  初始化方法會宣告子模組。
2.  子模組是複雜AI系統的一部分。

#### 前向方法

1.  前向方法定義程式邏輯。
2.  這個邏輯可以用迴圈來表示。

### 策略和語言模型

#### 策略

1.  策略是用於生成搜索查詢和答案的方法。
2.  它們能夠改善品質，尤其是在多層次的情況下。

#### 語言模型

1.  語言模型是一種用於理解自然語言的技術。
2.  它可以用來生成文本和回答問題。

**Meta-Programming**
=====================

### 問題描述

*   **Tensors**: 
    *   可以接受的類型
    *   給出的類型
*   **Inference Strategies**: 
    *   這些策略可以被抽象化並定義在這些簽名上
    *   能夠表達這些行為

### 問題意義

*   **Abstraction**: 
    *   如何寫程式碼
*   **系統運作**: 
    *   如何讓這個抽象化的程式碼實際運作並能被部署

### 解決方案

#### 第一步驟: 基本提示轉換

*   **Predictors**: 
    *   這是一個基本提示
    *   可以通過預先設定好的適配器和預測器來轉換
*   **Adapters**: 
    *   這是用於格式化提示的模組
    *   可能是聊天模型或指令模型

#### 第二步驟: 提示轉換

*   **Basic Prompt**: 
    *   基本提示的樣式
    *   可以通過預先設定好的適配器和預測器來轉換
*   **Query Format**: 
    *   這是用於格式化提示的模組
    *   可能是聊天模型或指令模型

### 結論

*   **Meta-Programming**: 
    *   這是一種抽象化程式碼的方法
    *   可以通過適配器和預測器來轉換成基本提示
*   **系統運作**: 
    *   這需要一個完整的系統架構
    *   包括適配器、預測器和基本提示

**Optimizers in Compound AI Systems**
=====================================

### Introduction

*   **Compound AI systems**: A system that combines multiple modules or prompts to achieve a specific task.
*   **Optimizers**: Algorithms used to optimize the performance of compound AI systems.

### Role of Optimizers

*   Take an initial prompt and the whole program as parameters
*   Look at them as variables that can be tinkered with to maximize a metric
*   Example: Using MIPROv2 optimizer in DSPy to improve accuracy on a given strict metric

### Examples

#### Trivial Compound AI System

*   A system that takes input and predicts output without optimization
*   Results:
    *   GPT 3.5: 33% accuracy
    *   Llama 2 model: lower accuracy

#### RAG System

*   A decomposition-based system for factual tasks
*   Potential improvement over trivial compound AI system

### Optimizers in Compound AI Systems

*   **MIPROv2**: An optimizer that can improve performance on a given strict metric
*   **Adam** and **RMSProp**: Other optimizers that can be used to improve performance
*   Example: Using MIPROv2 to improve accuracy on a multi-hop question answering task

**小型模型的優勢**
================

*   一個小型模型可以在某些情況下比一個更大的模型，具有較為複雜架構或未經優化的模型表現得更好。
*   但是，大型模型仍然能夠保留一定的優勢。

**多跳躍式合成AI系統**
------------------------

*   可以通過迭代程式並建立一個多跳躍式合成AI系統來提升性能。
*   這種方法可以在大型模型和開放模型上都取得顯著改善。

**優化器的空間**
-----------------

*   我們可以使用優化器來更新權重，從而進行微調。
*   這樣一來，我們就能夠在一個巨大的空間中實現強化學習。

**小型模型的模仿**
-------------------

*   我們可以通過使用優化器來使小型模型模仿更大的模型。
*   這種方法可以讓我們在短時間內取得競爭力，甚至超越當前的前沿模型。

**未來的研究方向**
------------------

*   我們將會探索優化器空間中的選擇和效果。
*   我們將會嘗試找到哪些選擇能夠提升性能，並且哪些選擇是無效的。

**使用程式**
================

### 程式輸入和評估
-------------------

*   **輸入**: 提供多個輸入值
*   **評估指標**: 依據輸入值評估結果的好壞
*   **評估方式**: 可以是簡單的正確答案檢查, 或者是對程式進行評估

### 收集模組輸出和更新程式
---------------------------

*   **收集模組輸出**: 使用評估指標收集每個模組的輸入和輸出
*   **更新程式**: 使用收集的輸出來更新程式

### 使用範例進行優化
-------------------

*   **使用範例**: 將過去成功的範例加入程式中, 作為參考
*   **探索範例**: 進一步探索哪些範例可以用於優化程式
*   **智能選擇**: 智能地選擇哪些範例可以用於優化程式

### 使用語言模型進行指導
-------------------------

*   **使用語言模型**: 將收集的範例提供給語言模型, 並要求它們提供建議
*   **指導**: 使用語言模型的建議來優化程式

**DSPy**
================

### 介紹

*   **DSPy** 是一個用於表達 AI 系統的程式語言。
*   它能夠讓使用者以更高層次的抽象來撰寫程式碼。

### 相關應用

#### MEDIQA 競賽

*   2023 年，多倫多大學參與了 MEDIQA 競賽，並贏得了比其他參賽學校和團隊還要好的 20 分差距。
*   他們使用 **DSPy** 和 **MIPRO** 進行程式碼優化。

#### 自殺偵測任務

*   馬里蘭大學的研究人員在自殺偵測任務中使用 **DSPy**，並取得了 40% 到 50% 的最佳結果。
*   他們的研究成果被發表在一篇論文中。

### 相關概念

#### MIPRO

*   **MIPRO** 是一個用於程式碼優化的方法。
*   它能夠幫助使用者找到最佳的程式碼組合。

#### Prompt Optimizers

*   **Prompt Optimizers** 是一個用於優化程式碼提示的工具。
*   它能夠幫助使用者找到最佳的程式碼提示。

**Optimizing Language Model Programs**
=====================================

### Introduction

* **IReRa**: A system for classifying with language models
* **STORM**: Generates Wikipedia articles from a topic
* **DSPy**: A framework for building and optimizing language model programs

### Problem Setting

* Given:
	+ Inputs: Examples of a task (e.g. questions)
	+ Developer-built language model program
* Goal: Optimize the language model program to maximize a specific metric

### Key Concepts

* **Multi-stage Language Model Programs**: A program that consists of multiple modules, each with its own function and parameters
* **Optimizing Instructions and Demonstrations**: The process of optimizing the language model program to achieve better performance on a specific task

### Important Points

* **Defining the Metric**: It's essential to explicitly define what metric you're trying to maximize
* **Independent Optimization**: Optimizing the language model program in a way that's independent of the prompts, so you can explore both axes modularly
* **Abstraction Forces Modularity**: The abstraction of the problem forces you to optimize the program in a modular and independent way

### Related Concepts

* **Labels**: Some metrics require labels, while others don't
* **Context Retrieval**: The process of retrieving context from earlier loops or modules
* **Evaluation Metrics**: Different metrics for evaluating the performance of the language model program

**Prompt Optimization**
=======================

### 問題描述

* 無法存取模型權重或日誌概率
* 需要快速迭代和高級別的自然語言空間API
* 想要最小化輸入數量和模型調用次數

### 假設與限制

* 假設無法存取模型權重或日誌概率
* 假設不需要中間指標或標籤
* 需要在預算有限的情況下工作
* 想要最小化輸入數量和模型調用次數

### 問題類型

1. **Prompt Exploration**
	* 如何探索長的組合式字串空間，尤其是沒有梯度的情況下？
	* 如何在不調用模型太多次的情況下進行探索？
2. **Module Interaction**
	* 如果有許多模塊，並且正在改變各個部分，如何知道哪些改變導致了進步或損害？

### 重要概念

* **Prompt Optimization**: 這是最強大的方法之一
* **Fine-tuning**: 需要使用這兩種方法才能取得最佳表現

**Blame Assignment**
=====================

### Method 1: Bootstrapping Examples

* **Simplest approach**: Generate a few-shot examples by running a dumb version of the program to build examples and then search over that space.
* **Iteration**: Take better programs, build even better models, use larger models to build examples.
* **Compositional space**: Very large compositional space.

### Method 2: Prompt Optimization

* **Assumptions**:
	+ Labels (inputs and outputs)
	+ One prompt
	+ No program involved
* **Goal**: Optimize the prompt to get a desired output
* **Research literature**: Rich, concurrent research under stronger constraints

### Method 3: Program-Based Approach

* **Tracking inputs and outputs**: Track the inputs and outputs of modules in the program.
* **Generating search queries**: Generate search queries based on the program's outputs.
* **Evaluating answers**: Evaluate the answers generated by the program and keep the trajectory if it meets the metric criteria.

### Key Concepts

* **Blame assignment**: Assigning blame to specific parts of a system or program
* **Bootstrapping examples**: Generating examples through self-execution of a program
* **Prompt optimization**: Optimizing input prompts to get desired outputs

**Optimization through Prompting (OPRO)**

### 什麼是 OPRO?

*   **定義**: Optimization through Prompting 是 DeepMind 的一種方法，用於探索和優化模型的輸出。
*   **原理**: 這個方法通過在輸入前加上一個前綴，來導引模型產生預期結果。

### OPRO 的工作流程

1.  **輸入前綴**: 將輸入前綴加到原始輸入中。
2.  **生成變體**: 根據輸入前綴生成多個輸出變體。
3.  **評估變體**: 評估每個輸出變體的效果。
4.  **選擇最佳變體**: 選擇最好的輸出變體。

### 對語言模型的應用

*   **簡單方法**: 使用協調漲升法來優化語言模型的輸出。
*   **步驟**:
    1.  **固定其他模塊**: 固定除一個模塊外的所有模塊。
    2.  **生成變體**: 根據輸入前綴生成多個輸出變體。
    3.  **評估變體**: 評估每個輸出變體的效果。
    4.  **選擇最佳變體**: 選擇最好的輸出變體。

### 問題和限制

*   **成本高昂**: 每次優化一個模塊時，需要重新執行整個程式，這是非常耗資源的。
*   **假設過於寬泛**: 這種方法假設最佳選擇在任何給定的階段都是最好的，這可能不是真實的情況。

**使用語言模型時的最佳實踐**
=====================================

### 不要過早優化

*   **不要只看表面**: 生成搜尋查詢時，盡量避免只看字面的意思，而是嘗試理解背後的意圖。
*   **考慮多種可能性**: 搜尋查詢可能有多種解釋，例如 SQL 查詢、Google 搜索或資料庫查找等。

### 提供上下文資訊

*   **提供完整的程式設定**: 對於語言模型程式，提供完整的程式設定和背景資訊，以幫助模型更好地理解使用者的需求。
*   **使用示範程式碼**: 使用示範程式碼來提供程式設定和背景資訊，幫助模型更好地理解使用者的需求。

### 避免過早優化

*   **不要只看表面**: 生成搜尋查詢時，盡量避免只看字面的意思，而是嘗試理解背後的意圖。
*   **考慮多種可能性**: 搜尋查詢可能有多種解釋，例如 SQL 查詢、Google 搜索或資料庫查找等。

### 使用 Oracle 語言模型

*   **使用 Oracle 語言模型**: Oracle 語言模型可以提供更強大的能力，可以幫助模型更好地理解使用者的需求。
*   **提供完整的程式設定**: 對於語言模型程式，提供完整的程式設定和背景資訊，以幫助模型更好地理解使用者的需求。

### 提供上下文資訊

*   **提供完整的程式設定**: 對於語言模型程式，提供完整的程式設定和背景資訊，以幫助模型更好地理解使用者的需求。
*   **使用示範程式碼**: 使用示範程式碼來提供程式設定和背景資訊，幫助模型更好地理解使用者的需求。

**Bootstrap Few-Shot**
=======================

### 概念

* **Few-shot learning**: 使用少量訓練樣本進行學習
* **Bootstrapping**: 利用少量資料建立模型，然後使用該模型來擴展資料集

### 策略一：建構範例並在其中搜索

* 建立範例以供模型學習
* 搜索範例以找到最佳解決方案

### 策略二：提供模型更多的基礎知識

* 將程式碼呈現給模型，使其能夠理解程式碼的意義
* 利用語言模型來建構程式碼的代表性

### 其他想法

* 使用標準文獻中的隨機指令作為模擬器
* 最大化系統的多樣性
* 將範例和基礎知識結合使用以達到最佳效果

**MIPRO Optimizer**
================

### 步驟

1. **Bootstrapping**: 建立候選指令和示範
	* 使用語言模型程式建立候選指令
	* 依據候選指令建立示範
2. **Surrogate Model**: 建立預測配置品質的模型
	* 基於超參數優化文獻中的方法
	* 用於樣本候選指令和示範組合
3. **Bayesian Optimizer**: 選擇最佳候選指令和示範組合
	* 使用收集函數來預測最佳組合
	* 依據最佳組合評估程式品質

### 模組

1. **Language Model Program**
	* 兩個模組：一為指令描述，另一為示範列表
	* 每個模組有兩個參數：指令描述和示範列表
2. **Surrogate Model**
	* 預測配置品質的模型
	* 用於樣本候選指令和示範組合

### 重要概念

* **Credit Assignment**: 分配責任至各模組
* **Hyperparameter Optimization**: 超參數優化文獻中的方法
* **Surrogate Model**: 預測配置品質的模型

**Optimizing Instructions for AI Systems**
=============================================

### Conceptual Understanding

* **Surrogate Model**: A model that learns from the performance of a surrogate (a simpler version) to improve its own performance.
* **Acquisition Function**: A function that determines which combinations to try next based on their potential improvement.

### Process of Optimization

1. **Sampling and Scoring**: Sample 30 combinations, get a score, and then use that score to update the surrogate model.
2. **Repeating the Process**: Repeat this process until a good combination is found.
3. **Improvement Over Time**: The surrogate model gets smarter over time, proposing better combinations.

### Comparison of Optimizers

* **Off-the-Shelf Optimizers**: Using powerful optimizers like yes optimizing or off-the-shelf things.
* **Human-written Prompts**: Writing prompts by hand to compare with optimized results.
* **Benchmarking**: Trying to think of ways to benchmark different optimizers against each other.

### LangProBe Benchmark

* **Language Model Program Benchmark**: A benchmark that has tasks like multi-hop stuff, classification, inference, etc.
* **Tasks with Multiple Modules**: Some tasks have two modules, some have four modules, and some have one module.
* **Results on Test Set**: Looking at optimizing instructions only through module level OPRO without grounding and with grounding.

### Key Findings

* **Optimizing Instructions vs. Basic Adapter**: Optimizing instructions can help quite a bit compared to using a basic adapter.
* **Overfitting**: Sometimes, optimizing instructions overfits to the training set if it's really small, making it worse.
* **Struggling with Tasks**: Optimizing instructions struggles with many tasks to optimize.

**自然語言程式設計**
=====================

### 一些關鍵概念：

*   **MIPRO**: 做少量指示優化的程式
*   **DSPy**: 允許使用抽象來做自然語言程式設計
*   **深度神經網路**: 用於模型預測
*   **程式控制**: 使用程式碼來達成目標

### 結論：

#### 重要的教訓：

1.  **複合人工智慧系統**：程式可以比使用深度神經網路更準確、可控和透明。
2.  **宣告性程式**: 使用程式碼來達成目標，可以比寫大量的程式碼更有效率。

#### 結論：

*   **自然語言程式設計**：使用抽象來做自然語言程式設計，可以讓程式設計更加簡單和有效率。
*   **程式控制**: 使用程式碼來達成目標，可以比使用深度神經網路更準確、可控和透明。

**DSPy**
================

### 介紹

*   **[59:43] 和探索這個空間。**
*   **[59:44] 而且他們在任何個別建議上都很差。**

### DSPy 的實用性

*   **[59:48] 在大規模搜索中，DSPy確實可以找到一些東西。**
*   **[59:51] 這些東西在某些情況下甚至超越了手動方法。**
*   **[59:58] DSPy 的真正力量在於它能夠釋放你對每個模組的選擇限制。**

### 自然語言程式設計

*   **[60:00] DSPy 能夠讓你直接探索複合 AI 系統。**
*   **[60:07] 這樣你就能從迭代和連接模組中得到更多的價值。**

### DSPy 的優點

*   **[60:12] DSPy 能夠幫助你找到正確的目標。**
*   **[60:16] 這在許多情況下並不明顯。**

### 自然語言程式設計的挑戰

*   **[60:21] 手動提示工程和推斷時間策略往往很模糊。**
*   **[60:35] 什麼是 chain-of-thought 呢？**

### DSPy 的實用性

*   **[60:40] DSPy 能夠提供可組合的預測器。**
*   **[60:45] 這些預測器能夠根據簽名進行元編程。**

### 自然語言程式設計的優點

*   **[61:00] 手動提示工程可以被抛棄。**
*   **[61:02] 你就能使用最佳化的程序。**

### DSPy 的應用

*   **[61:04] DSPy 在生產和開源中已經得到廣泛使用。**
*   **[61:06] 連 JetBlue、Databricks、Walmart、VMware、Replit、Hayes Labs、Sephora 和 Moody's 都在使用它。**

### 自然語言程式設計的挑戰

*   **[61:13] 在許多情況下，自然語言程式設計的最佳方法並不明顯。**
*   **[61:16] 這需要通過實驗和測試來找到。**

**DSPy**
================

### **強大功能**

*   能夠獨立地修改和合成四到五個方面的程式：
    *   Signatures
    *   Optimizers
    *   Adapters
    *   Metrics
    *   Inference-time strategies

### **開放研究**
------------------

*   **目標**: 啟用開放研究領域再次領導人工智慧的進展。
*   **優點**:
    +   可以更好地控制程式的開發和應用。
    +   能夠促進開源研發。

### **模組化**
----------------

*   **概念**: 使用模組化來分解程式，讓每個部分都能獨立地修改和合成。
*   **優點**:
    +   可以更好地控制程式的開發和應用。
    +   能夠促進開源研發。

### **實際案例**
-----------------

*   **RL-based prompt optimizer**: 使用強化學習來改善程式的輸出。
*   **Inference-time strategy**: 使用預測模型來優化程式的執行速度。

**模型設計的變遷**
=====================

### **閉合式模型設計**

#### **現代閉合式模型設計**

*   **定義**:CLOSED (Customer-Defined, Owned, Operated, and Maintained) 模型設計是一種企業自行定義、擁有、運營和維護的模型設計。
*   **特點**:
    *   企業完全控制模型設計
    *   可以根據業務需求進行調整
    *   適合於需要高度靈活性和可定制性的情況

#### **優缺點**

##### **優點**

*   高度自主性和可定制性
*   透過企業內部資源實現控制和維護

##### **缺點**

*   需要大量資源和人力投入
*   可能導致複雜度增加和成本增高

---
## 參考資料
- 原始影片：[CS 194/294-196 (LLM Agents) - Lecture 5, Omar Khattab](https://youtube.com/watch?v=JEMYuzrKLUw)
