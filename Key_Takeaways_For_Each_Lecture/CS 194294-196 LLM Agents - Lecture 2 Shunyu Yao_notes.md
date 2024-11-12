# CS 194/294-196 (LLM Agents) - Lecture 2, Shunyu Yao

## 課程筆記

**LLM Agents**
================

### 什麼是 LLM Agent?

#### 定義

*   **智能系统**: 能够与某种环境进行交互的系统。
*   **环境**: 可能是物理环境（如机器人或自动驾驶汽车）或数字环境（如视频游戏或iPhone）。
*   **智能**: 在 AI 历史中，定义可能会随着时间而改变。

### 什麼是 LLM？

#### 定義

*   **LLM**: 语言模型。
*   **LLM Agent**: 使用 LLM 的智能系统，可以与某种环境进行交互。

### 未來方向
-----------------

*   **未來發展**: LLM Agents 可能会用于各种应用，例如客服、内容生成等。

**LLM Agent**
================

### 一級定義: 文本代理人 (Text Agent)

*   定義: 代理人與環境互動, 其中文本和觀察均為語言形式。
*   例子: 早期的聊天機器人 (Chat Bots) 如 ELIZA。

### 二級定義: LLM 代理人 (LLM Agent)

*   定義: 文本代理人, 同時使用 LLMs 作為行動。
*   例子: 使用 LLMs 的聊天機器人。

### 三級定義: 理解代理人 (Reasoning Agent)

*   定義: 代理人使用 LLMs 進行推理, 再作出行動。
*   例子: 未來的可能應用。

**文本代理人的限制**
------------------------

*   規則基礎的代理人:
    *   每個新領域需要新的規則
    *   不適合複雜的領域
*   使用 RL 的代理人:
    *   需要可擴展的獎勵信號
    *   需要大量訓練

**LLMs (Large Language Models)**

### Promise of LLMs

*   **Revolutionize text agent**: LLMs are trained on massive text corpora and can be prompted to solve various new tasks.
*   **Generality and feature learning phenomena**: This kind of generality will be really exciting to build agents.

### Brief Overview of LLM Agents

#### Historical View (Simplified)

1.  **LLM in 2020**: The beginning of LLM is GPT-3.
2.  **Exploration across different tasks**:
    *   Reasoning tasks: symbolic question answering and so on.
    *   Acting tasks: games, robotics, and so forth.
3.  **Convergence of paradigms**:
    *   Reasoning paradigm
    *   Acting paradigm
4.  **Reasoning Agent**: A new paradigm that's quite different from previous agents.

#### New Applications and Methods

1.  **New applications**:
    *   Web interaction
    *   Software engineering
    *   Scientific discovery
2.  **New methods**:
    *   Memory
    *   Learning
    *   Planning
    *   Multi-agent

### Paradigm of Reasoning and Acting

*   **Paradigm of reasoning**: A way of solving problems that involves logical thinking.
*   **Paradigm of acting**: A way of solving problems that involves taking actions.

### History Discussion (Simplified)

1.  **Focus on one task: question answering**:
    *   A very intuitive task
    *   One of the most useful tasks in NLP

2.  **Challenges in question answering**:

    *   Difficulty in directly outputting answers
    *   Need for reasoning and chain of thought reasoning

**語言模型的局限性**
=====================

### 問題回答的挑戰

*   **知識更新**: 如果訓練語言模型的時間點過去，可能會導致錯誤的答案。
*   **計算能力**: transformers 無法處理複雜的數學問題。

### 解決方案

#### 1. **Retrieval-Augmented Generation (RAG)**

*   **概念**: 使用額外的資源（如 Wikipedia）來增強語言模型的回答能力。
*   **流程**:
    *   利用 retriever 搜尋相關資訊。
    *   將搜尋結果與語言模型的上下文結合。

#### 2. **工具使用**

*   **概念**: 使用特殊令牌來呼叫外部工具或 API，增強語言模型的回答能力。
*   **例子**:
    *   使用 calculator 令牌計算數學問題。
    *   使用 Wikipedia 令牌查詢知識。

### 結論

語言模型有其局限性，但透過 RAG 和工具使用等解決方案，可以增強其回答能力。

**Language Model**
================

### 問題描述

*   有沒有能夠生成這樣的文本的博客文章或維基百科條目？
*   如果要讓語言模型生成這樣的文本，需要在特定格式下進行微調。
*   這種微調過程相當困難。

### 問題延伸

*   如果需要同時具備推理和知識呢？
*   人們已經提出許多不同的解決方案。
*   例如，可以將推理鏈和知識檢索結合在一起，或生成跟進問題等。

### 解決方案

*   不過，我們不需要深入探討所有方法。
*   我只是想指出，在當時的情況下，情況相當散亂。
*   單一任務叫做 QA，但其實是多個不同的任務。
*   有許多不同的基準測試，挑戰語言模型的方式各不相同。

### 反思

*   我們是否能夠找到一個簡單而統一的解決方案？
*   如果要達到這點，我們需要超越個別任務或方法。
*   需要更高層次的抽象。
*   這種抽象是推理和行動。

### 推理鏈

*   這是一種很直觀且靈活的方式，增強測試時間的計算能力和推理能力。
*   但如果只使用推理鏈，你就沒有外部知識或工具。

### 行動

*   這是另一個抽象概念，因為你假設有個代理。
*   這代理可以與外部環境互動，例如知識檢索、搜索引擎、計算器等。
*   這種方式增強了知識和計算能力，但沒有推理能力。

### ReAct

*   這是一種新的抽象概念，結合了推理鏈和行動。
*   這可以增強語言模型的推理和行動能力。

**ReAct**
================

### 重要概念

*   **Reasoning and Acting**: Two paradigm for language models
*   **One-shot prompting**: Using a single example to generate thought and action
*   **Few-shot prompting**: Using a few examples to generate thought and action
*   **Fine-tuning**: Adjusting the model with many examples

### ReAct 的概念

#### 思考和行動的生成

*   使用語言模型生成思考和行動
*   行動會觸發觀察
*   觀察會被追加到語言模型的上下文中
*   語言模型會根據新的上下文生成新的思考和行動

#### 促進和調整

*   使用單一範例（one-shot prompting）
*   使用幾個範例（few-shot prompting）
*   進一步調整模型（fine-tuning）

### 實際應用

#### 問題解決

*   使用語言模型回答問題
*   例如：如果我有 $7 trillion, 可以買 Apple, NVIDIA, 和 Microsoft?

#### 思考和行動的生成

*   語言模型會根據 prompt 生成思考和行動
*   行動可能是 Google 搜尋或直接提供答案

**ReAct Paradigm**
================

### 什麼是 ReAct?

*   **ReAct**: 是一個使用搜索引擎作為計算器來解決問題的方法。
*   **市場資產**: 是指公司的總市值。

### 如何運用 ReAct?

#### 步驟一: 找到市場資產

1.  使用搜索引擎查找市場資產
2.  將市場資產加總

#### 步驟二: 進行計算

*   使用搜索引擎作為計算器
*   加總市場資產
*   得出結果

### ReAct 的優點

*   **直覺**: 使用者可以輕鬆理解和運用 ReAct。
*   **適應性**: ReAct 可以根據情況進行調整和重新規劃。

### 進一步的應用

*   **工程任務**: ReAct 可以用於解決各種工程任務，只要提供不同的例子和工具即可。
*   **超越 QA**: ReAct 的理念可以用於解決任何任務，不僅限於質量保證。

**ReAct**
================

### 什麼是 ReAct

*   **定義**: ReAct 是一個將任務轉換為文字遊戲的方法。
*   **原理**: 利用語言模型和控制器來轉換語言動作為鍵盤操作。

### ReAct 的應用範圍

*   **超越問答系統**: ReAct 可以解決更複雜的任務，遠超問答系統。
*   **結合強化學習、機器人學和視頻遊戲等領域**: ReAct 的概念源於這些領域的研究。

### ReAct 的問題

*   **直接映射觀察到行動的困難**: 有時很難直接將觀察轉換為行動，因為可能沒有見過該領域或需要思考。
*   **模仿而非真正解決任務**: 如果沒有思考能力，ReAct 只會試圖模仿觀察到行動的映射。

### ReAct 的優點

*   **添加思考行為**: ReAct 加入了一種新的行為——思考，可以用於任何任務。
*   **幫助計劃和重新規劃**: 思考行為有助於計劃、跟蹤和重新規劃任務。

### ReAct 的普遍性

*   **適用於多個任務**: ReAct 是一個通用的模式，適用于各種任務。
*   **系統性地解決問題**: ReAct 可以系統地解決複雜的任務。

**Reasoning Management**
=======================

### **Abstraction**

*   Everything from video game to AlphaGo to autonomous car has an action space defined by the environment.
*   Action space is fixed, e.g., left, right, up, down in Atari games.

### **Augmented Action - Reasoning**

*   Language agent or LLM agent has an augmented action called reasoning.
*   Reasoning can be any language and is an infinite space.
*   It doesn't change the environment but changes your own context and memory.
*   Follow-up actions are based on changed context and memory.

### **Reasoning Management Paradigm**

*   Different from paradigm of only doing reasoning or only doing action.
*   Reasoning has a special property as it's an internal action for agents with an infinite space of language.
*   This new paradigm is different because reasoning is an internal action that changes your own context and memory.

### **Methodological Side - Long-term Memory**

*   Reasoning agent can also think and have long-term memory.
*   External environment (e.g., video game, Google search engine) vs. internal context window of the language model.
*   Context window is append-only, only new tokens can be appended to it.

### **Progress and Future Directions**

*   There's a lot of progress in reasoning management paradigm and more methods are being developed.
*   Long-term memory is one aspect that needs to be covered.

**長期記憶**
================

### 定義

*   長期記憶是指能夠持續存在於時間上的記憶。
*   這種記憶與短期記憶相比，能夠持續更久，並且不容易被干擾。

### 特點

*   **持續性**:長期記憶能夠持續存在於時間上，不會因為時間的流逝而消失。
*   **穩定性**:長期記憶相比短期記憶更穩定，不容易被干擾或改變。

### 例子

*   人類的日記：人們可以通過寫日記來記錄重要事件、經驗和知識，這些信息能夠持續存在於時間上。
*   數學家對數學問題的解決方案：數學家可以通過寫下解決方案的步驟和結果來記錄自己的經驗和知識，這些信息能夠持續存在於時間上。

### 長期記憶的應用

*   **學習**:長期記憶能夠幫助人們在學習過程中記住重要資訊和經驗。
*   **工作流程**:長期記憶能夠幫助人們記住工作流程、步驟和結果。

### 長期記憶的缺點

*   **記憶容量**:長期記憶的記憶容量有限，不能夠記住所有的資訊。
*   **查找難度**:長期記憶中的資訊可能需要花費時間來查找和回憶。

**長期記憶**
================

### **什麼是長期記憶**

*   長期記憶是一種可以儲存大量資訊的能力。
*   透過長期記憶，可以在未來的時間點讀取和回顧已經學習的知識。

### **如何使用長期記憶**

*   當你重新撰寫程式碼時，你可以直接從長期記憶中讀取資訊。
*   透過反思和檢視成功或失敗的經驗，可以進一步改善自己的能力。

### **與傳統學習方法的差異**

*   長期記憶不使用單一的獎勵機制（scalar reward）。
*   可以使用程式碼執行結果、編譯器反饋或教師的回饋等多種資訊來進行學習。
*   學習不是透過梯度下降，而是通過更新語言和記憶體中的知識。

### **長期記憶的應用**

*   可以用於程式碼撰寫、遊戲玩法等多個領域。
*   透過長期記憶，可以避免重複地嘗試相同的事情，並且可以快速改善自己的能力。

**長期記憶**
================

### 定義

*   長期記憶是指能夠存儲在腦海中的資訊，能夠在需要時被回憶起來。
*   這種記憶可以幫助我們了解自己和他人。

### 例子

*   你可以透過檢視日曆，得出對其他人的結論。
*   你可以反思並得出自己的結論。
*   這種知識能夠影響你的行為。

### 相關概念

*   **短期記憶**
    *   是指能夠暫時存儲在腦海中的資訊，通常只有幾秒鐘的時間。
    *   可以幫助我們理解現在的情況。
*   **語言模型**
    *   是一個可以學習和改善自己能力的系統。
    *   可以透過修改參數或寫新的程式碼來改善自己。

### 問題

*   什麼使得外部環境與內部記憶不同？
*   如果代理人打開Google Doc並寫下東西，是那種形式的記憶？是行動還是長期記憶？

**參考資料**
================

*   CoALA：一個可以表達任何代理人的系統。

**物理代理人與數位代理人**
=====================================

### 定義外部與內部

*   **物理代理人**: 如同人的代理人或自主汽車，很容易定義外部和內部。
    *   外部: 不在皮膚之外的東西
    *   內部: 在皮膚之內的東西
*   **數位代理人**: 如何定義外部與內部呢?

### 長期記憶與短期記憶

*   **長期記憶**: 10,000,000 個令牌的語言模型是否仍然是長期記憶?
*   **短期記憶**: 人類心理學和神經科學定義了這些術語。

### 代理人歷史

#### LLM代理人的簡史

*   **符號AI**: 程序化規則來互動環境
*   **深度學習**: 從 Atari 到 AlphaGo 等等
*   **LLM代理人**: 最近才出現的新一代代理人

### 代理人類型比較

#### 三種代理人的差異

*   **符號AI代理人**:
    *   使用程式化規則來互動環境
    *   代表性的例子: 對話系統
*   **深度學習代理人**:
    *   使用深度神經網路來訓練模型
    *   代表性的例子: LSTM-DQN
*   **LLM代理人**:
    *   使用語言模型來處理任務
    *   代表性的例子: 10,000,000 個令牌的語言模型

**深度強化學習 (Deep Reinforcement Learning, DRL)**
=============================================

### **符號狀態**

*   [40:28] 符號狀態是用來描述觀察的抽象表現。
*   [40:30] 該狀態用於推導行動。

### **if-else規則**

*   [40:34] if-else規則是一種簡單的程式設計方式，用於根據不同條件執行不同的動作。

### **符號狀態與深度強化學習**

*   [40:36] 符號狀態與深度強化學習相比，後者更抽象。
*   [40:45] 深度強化學習的觀察可以是任何形式，包括像素、文本等。

### **符號狀態與語言代理**

*   [41:19] 語言代理使用語言作為中間表示法，用於處理觀察到行動。
*   [41:24] 這種方法更接近人類的思考方式。

### **符號狀態與深度強化學習的差異**

*   [41:46] 符號狀態和深度強化學習都需要大量努力來設計或訓練。
*   [42:07] 但深度強化學習的模型通常是任務特定的，不能重用。

### **語言代理的優點**

*   [42:31] 語言代理可以使用既有的知識庫（LLMs），不需要大量努力來設計或訓練。
*   [42:38] 這使得語言代理更具普遍性和可重用性。

### **思考與符號狀態的差異**

*   [43:07] 思考可以無窮無盡地延伸，而符號狀態和深度強化學習的模型通常具有固定的大小。
*   [43:10] 這使得思考在推理時具有無限的可擴展性。

**長期記憶**
================

### **什麼是長期記憶**

*   長期記憶是人腦中儲存的資訊，能夠在長時間內保存和回憶。
*   這種記憶與短期記憶相比，更穩定且持久。

### **長期記憶的特點**

*   能夠在長時間內保存和回憶
*   穩定且持久

### **什麼是語言模型**

*   語言模型是一種人工智能技術，能夠理解和生成自然語言。
*   這種模型通過學習大量文本資料，來預測下一個字或詞的可能性。

### **語言模型的應用**

*   題目回答
*   遊戲
*   數據分析
*   文字生成

### **什麼是數位自動化**

*   數位自動化是一種技術，能夠幫助人們完成繁瑣且重複的任務。
*   這種技術通過語言模型等工具，來提高工作效率和減少錯誤。

### **語言模型的限制**

*   只能處理簡單的任務
*   不具備深度思考能力

### **新型態的語言模型**

*   能夠理解和生成自然語言
*   可以完成複雜的任務
*   具有深度思考能力

**WebShop環境**
================

### 特點

* 可以輸入搜尋查詢
* 可以檢查不同產品並重新搜尋
* 可以給予獎勵評估

### 操作流程

1. 輸入搜尋查詢
2. 檢查不同產品
3. 重新搜尋
4. 給予獎勵評估 (0-1)

### 相關概念

* **強化學習環境**：基於文字的觀察和行動
* **WebShop**：第一個大規模、複雜的環境，基於實際網路數據
* **SWE-Bench**：軟體工程任務，基於 GitHub repo 和 issue

### 其他相關概念

* **GridWorld**：一個簡單的環境，用於強化學習
* **ChemCrow**：使用推理 LLM 代理來尋找新染色體的任務

**ReAct Paradigm**
================

### **什麼是 ReAct?**

*   **ReAct** 是一個新的 AI 模型架構，結合了推理和行動的能力。
*   這個模型可以從大量數據中學習，並使用工具如 Python 或互聯網來分析並提出新化學物質的建議。

### **ReAct 的優點**

*   **物理空間延伸**：ReAct 模型可以將行動空間延伸到物理空間，讓它們能夠在實驗室中進行實驗和合成。
*   **反饋機制**：ReAct 可以從實驗室獲得反饋，並使用這些反饋來改進自己。

### **ReAct 的應用**

*   **創新化學物質**：ReAct 模型可以幫助開發新的化學物質。
*   **科學探索**：ReAct 可以幫助科學家進行更深入的研究和實驗。

### **簡單是好的**

*   **簡單意味著普遍性**：一個簡單的模型往往能夠應用在多個領域。
*   **簡單是最好的研究**：一個簡單但有效的模型往往比複雜的模型更有價值。

### **簡單的挑戰**

*   **跳出個別任務**：要想簡化自己的模型，必須能夠跳出個別任務和數據點。
*   **思考在較高層次**：簡化的模型需要能夠思考在較高層次。

### **結合簡單與熟悉**

*   **既要簡單又要熟悉**：一個簡單但有效的模型必須既能夠簡化，又能夠熟悉個別任務和數據點。

**LLM Agents 的未來**
=====================

### 历史和抽象思维

*   **学习历史的重要性**: 了解 LLM Agents 的发展史有助于我们更好地理解当前的技术局面。
*   **抽象思维的练习**: 学习其他学科有助于我们培养抽象思维能力，这对解决复杂问题至关重要。

### 未来方向

#### 五个关键话题

1.  **首要训练**
    *   如何训练模型为代理人服务
    *   数据来源的问题
2.  **接口**
    *   如何建立代理人的环境
3.  **健壮性**
    *   确保代理人在真实世界中有效工作的方法
4.  **人类**
    *   确保代理人与人类相互作用时有效工作的方法
5.  **基准**
    *   如何建立良好的基准

#### 未来展望

*   **多维度**: 未来的发展方向多样化，具有许多令人兴奋的可能性。
*   **低垂果实**: 有可能在当前阶段就能取得显著进展或创造一些基础性的成果。

**問題**: 資料不一致的問題
==========================

### 一、資料不一致的問題

*   **問題描述**
    *   [57:14] So it's not trained to do those things,
    *   [57:15] but then it's prompted to do those things.
    *   [57:17] So the performance is not optimal.
    *   [57:21] And one solution to do that is--
*   **解決方案**
    *   [57:24] one solution to fix this is you should train models, probability for agents.
    *   [57:30] And once you can do this, you can use those prompted agents to generate a lot of data.
    *   [57:36] And then you can use those data to fine-tune the model to be better at agents.

### 二、資料不足的問題

*   **問題描述**
    *   [57:53] is the predominant source of language model training, there is not a lot of self-evaluation kind of data.
    *   [58:01] People only give you a well-written blog post, but no one really releases all the thought process and action process of how to write the blog post.
*   **解決方案**
    *   [58:14] So you can actually prompt agents to have those trajectories, and you can train models on those things.

### 三、未來發展的方向

*   **問題描述**
    *   [58:30] internet data is running out. And how can we have the next trillion dollars to train models?
*   **解決方案**
    *   [58:41] This is very exciting and, I think, a very-- like, maybe not best analog is you can think of the synergy between GPU and deep learning.

### 四、接口的問題

*   **問題描述**
    *   [59:19] The second topic is interface. And in fact, human-computer interface has been a subject for decades.
*   **解決方案**
    *   [59:32] if you really cannot optimize the agent, you can optimize the environment.

### 五、未來發展的方向

*   **問題描述**
    *   [60:00] So it's a very concrete example. You can imagine, how can the agent search files in OS?
*   **解決方案**
    *   [60:11] So the human interface is actually an important factor for agents.

**Interface Design for Agents**
=====================================

### Introduction

* 使用 `LS` 和 `CD` 等命令的方式是人類的接口設計，但不是最佳的對於代理程式。
* 可以定義新的命令，例如 `Search`，並提供結果和下一步驟。

### Best Interface Design for Agents

* 根據 SWE-agent 研究發現，最好的方法是使用特定的 `search` 命令。
* 可以一次提供多個結果（例如 10 個），讓代理程式決定哪一個最重要。
* 這種設計可以幫助代理程式更有效率地搜索檔案。

### Interface Design for Humans vs. Models

* 人類的短期記憶有限，需要設計簡單易用的介面。
* 模型有較長的上下文窗口，可以一次處理多個結果。
* 設計合適的介面可以幫助代理程式更有效率地完成任務，並且了解人類和模型之間的差異。

### Human-in-the-Loop and Robustness

* 人類在迴路中的重要性和穩健性是研究的關鍵。
* 現有的基準測試與實際世界中的人們所關心的事務有很大差距。
* 例如，程式設計與單元測試是一個典型的代理任務，但現有的基準測試並不能完全反映出人類在這個過程中的重要性。

**Benchmarking Challenge**
==========================

### **Pass at K**

* What you care about is, can I solve it one time out of 10,000 times or 1,000 times or a million times?
* It's like solving Riemann hypothesis. You just need to do it once.

### **Robustness in Real World Jobs**

* Most jobs require robustness, not just passing at K.
* Customer service is an example, where reliability is key.
* If you fail one time, you might lose a customer.

### **Tau-bench**

* A recent work that calls for a different way of doing benchmarking.
* It's designed to test the ability to solve practical tasks reliably.
* The agent interacts with both backend API and user simulation.

### **Customer Service Task**

* The agent needs to interact with both backend API and user simulation.
* The trajectory might look something like this:
	+ Human might not give all information at beginning.
	+ Agent needs to prompt user for more information.
	+ Interaction over multiple turns is required.

### **Metric of Interest**

* You care about the ability to solve the task a thousand times out of a thousand times.
* Will I fail it one time out of a thousand times?
* If you fail, you might lose a customer.

**Pass@K**
================

### 概念

* **Pass@K**: 測量模型在多次嘗試下能夠正確解決任務的機率。
* **Robustness**: 型號在多次嘗試下能夠保持解決任務的能力。

### 問題

* 如果嘗試 10 次，能否至少一次解決任務？
* 測量模型的 Robustness 是否隨著嘗試次數增加而改善？

### 結果

* **Pass@K** 測量結果顯示，型號在多次嘗試下能夠保持解決任務的能力會下降。
* 即使是大型模型，也會出現類似的趨勢。

### 建議

* 需要更多努力將實際世界元素融入基準測試中。
* 這需要新的設定和指標。

### 未來展望

* 想像一下語言代理能夠取代的工作類型：
	+ 第一種任務：不需要高智慧，但需要 Robustness，例如簡單偵錯或客服。
	+ 第二種任務：需要與人合作。
	+ 第三種任務：需要完成困難任務，例如撰寫調查報告或發現新基因。

---
## 參考資料
- 原始影片：[CS 194/294-196 (LLM Agents) - Lecture 2, Shunyu Yao](https://youtube.com/watch?v=RM6ZArd2nVc)
