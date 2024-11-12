# CS 194/294-196 (LLM Agents) - Lecture 1, Denny Zhou

## 課程筆記

**大型語言模型代理人**
========================

### 教學團隊

*   **教授**: Dawn Song (UC Berkeley)
*   **助教**: Alex, Sehoon
*   **讀者**: Tara, Ashwin

### 課程內容

#### 大型語言模型的簡介

*   **大型語言模型**：能夠快速學習並產生文本輸出的模型
*   **下一個前沿技術**：使用大型語言模型作為推理和計畫的關鍵腦部，讓代理人能夠與外部環境互動、觀察環境並採取行動

#### 大型語言模型代理人的能力

*   **與外部環境互動**
    *   觀察環境
    *   取得資訊
    *   進行操作
*   **使用外部工具和資料庫**
    *   取得資訊
    *   進行分析
*   **多樣化的能力**
    *   能夠在不同的環境中運作
    *   能夠與不同類型的環境互動

#### 大型語言模型代理人的特點

*   **靈活性高**
*   **能夠學習和改進**
*   **能夠與人類互動**

### 結論

大型語言模型代理人是一種新興技術，具有多樣化的能力和靈活性。它們能夠與外部環境互動、觀察環境並採取行動，並且能夠學習和改進。這項技術將會在未來的發展中扮演重要角色。

**Agent**
================

### 重要概念

*   **Multi-Agent Collaboration**: 多個代理程式之間的合作和互動
*   **Task Decomposition**: 任務分解，將複雜任務分成更小的子任務
*   **Embodiment and Learning**: 身體化學習和環境反饋

### 重要挑戰

#### Reasoning and Planning

*   改善代理程式的推理和計畫能力
*   增強代理程式在複雜任務中的正確率

#### Embodiment and Learning

*   提升代理程式的身體化學習和環境反饋能力
*   增強代理程式對錯誤的恢復能力

#### Multi-Modal Understanding

*   提升代理程式對多種模式的理解能力
*   增強代理程式的自我改善能力

#### Safety and Privacy

*   保障代理程式的安全性和隱私性
*   避免代理程式受到攻擊和發出有害訊息

**課程概述**
================

* **課程目標**: 掌握控制代理行為、設計人機互動模式和讓機器服務人類需求的方法。
* **課程範圍**: 覆蓋代理框架各層級和領域的基礎知識。

**課程內容**
------------

### 第一部分: 基礎知識

#### 代理能力

* **推理能力**
* **規劃能力**
* **多模式理解**

#### 流行代理框架

* **設計代理應用程序**
* **使用流行代理框架**

### 第二部分: 應用領域

#### 軟件開發

* **工作流程自動化**
* **多模式應用**
* **企業應用**

### 第三部分: 安全性和倫理

* **代理安全性**
* **代理倫理**

**預期對於 AI 的發展**
-------------------------

* **解決難以解決的數學問題**
* **發現新科學理論**
* **解決 AGI 問題**

**機器學習的期待**
-------------------

* **能夠從少量範例中學習**
* **能夠使用資料效率方法**

**未來展望**
-------------

* **代理框架的進一步發展**
* **人機互動模式的改善**
* **安全性和倫理的關注**

**機器學習缺陷**
================

### 問題描述

*   **背景**: Denny Zhou 提到自己在幾乎 20 年前開始研究機器學習。
*   **問題**: 人類可以透過少數例子學習，而不是因為資料統計。

### 解決方案

#### 1. **簡單的玩具問題**

*   **最後字連接**: 給定一個人的名字，輸出是前名和後名最後字的連接。
    *   **範例**: Elon Musk 的輸出是 NK。

#### 2. **機器學習方法**

*   **缺陷**: 需要大量標記資料才能學習。
*   **質疑**: 是否該稱之為人工智慧 (AI)?

#### 3. **大型語言模型 (LLM)**

*   **定義**: 训練用於預測下一個字的模型。
*   **範例**: 給定文本 "AI 是未來"，輸出 "future"。

### 結論

*   **機器學習缺陷**: 需要大量標記資料才能學習簡單任務。
*   **質疑**: 是否該稱之為人工智慧 (AI)?

**訓練大型語言模型 (LLMs) 的基礎**
=====================================

### 一、使用多句子分享模型

*   可以使用所有網路上的文本進行訓練
*   讓模型學習人類語言的模式

### 二、訓練模型的過程

#### 1. 訓練模型的方式

*   讓模型學習創建下一個token的過程
*   可以使用任何輸入並觀察模型的輸出

#### 2. 模型預測下一個token

*   模型可以預測下一個token
*   可以將生成的token與原來的token合併

### 三、使用少量示範進行訓練 (Few Shot Prompting)

#### 1. 使用示範進行訓練

*   可以使用少量示範進行模型的訓練
*   這是通過將輸入和輸出合併並讓模型學習的過程

#### 2. 添加推理過程

*   可以在輸出前添加推理過程
*   這可以幫助模型更好地理解問題

### 四、結論

*   使用少量示範進行訓練是一種有效的方法
*   這可以幫助模型學習快速和準確地回答問題

**中間步驟**
================

### 中間步驟的重要性

*   **提前研究**: 中間步驟已經在文獻中被提出多年。
*   **Google DeepMind 的研究**: 2017 年, Google DeepMind 出版了一篇關於自然語言推理的論文, 其中使用了中間步驟來解決數學問題。

### GSM8K 資料集

*   **GSM8K 資料集**: 2021 年, OpenAI 出版了一個名為 GSM8K 的資料集, 這個資料集包含了每個問題後面的中間步驟和最終答案。
*   **使用 GSM8K**: 使用這個資料集來訓練 GPT3 模型。

### Google Brain 的研究

*   **Google Brain 的研究**: 2021 年, Google Brain 出版了一篇關於程式合成的論文, 其中使用了抽象符號來表示中間步驟。
*   **獨立發現**: 這個團隊獨立發現了類似的想法。

### Chain-of-thought Prompting

*   **Chain-of-thought Prompting**: 這是一種多步驟推理的方法, 其中使用了中間步驟來解決問題。
*   **結果**: 這種方法在各個 NLP 任務上都取得了令人驚嘆的效果。

### 結論

*   **中間步驟的重要性**: 無論是訓練、微調或提示, 提供包含中間步驟的範例給 LLMs, 它們都會產生包含中間步驟的回應。
*   **推理策略**: 是否有幫助於在範例中引入推理策略?

**工作團隊**
================

### **概念**

*   **最少提示 (Least-to-Most Prompting)**: 問題解決的方法，從簡單到複雜。
*   **分解 (Decomposition)**: 分解複雜問題為更容易解決的部分。

### **工作內容**

#### **例子**

*   **Elsa 和 Anna 的蘋果**: Elsa 有 3 個蘋果，Anna 有 2 個比 Elsa 多。一起有多少個蘋果？
*   **SCAN 任務 (SCAN Task)**: 分解自然語言指令，轉換為行動序列。
*   **CFQ 任務 (CFQ Task)**: 文字轉碼，另一項組合性推廣任務。

### **結果**

*   **99.7% 的準確率**: 使用最少提示方法，可以達到 99.7% 的準確率，只需使用 0.1% 的示範例子。
*   **動態最少提示 (Dynamic Least-to-Most Prompting)**: 對於 CFQ 任務，使用 1% 的數據，取得了比文獻中結果更好的效果。

### **相關概念**

*   **組合性推廣 (Compositional Generalization)**: 任務例子比訓練或提示例子更困難。
*   **動態最少提示 (Dynamic Least-to-Most Prompting)**: 對於 CFQ 任務，使用 1% 的數據，取得了比文獻中結果更好的效果。

**Chain-of-Thought Prompting**
=====================================

### 什麼是 Chain-of-Thought Prompting?

* **定義**: Chain-of-Thought Prompting 是一種技術，讓模型生成中間步驟來解決問題。
* **目的**: 這項技術的目的是幫助模型更好地理解和解決複雜的問題。

### Chain-of-Thought Prompting 的優點

* **提高模型的解決能力**: Chain-of-Thought Prompting 可以幫助模型生成中間步驟，從而提高其解決問題的能力。
* **改善模型的溝通能力**: 這項技術可以幫助模型更好地溝通自己的思維過程和推理結果。

### Chain-of-Thought Prompting 的實際應用

* **教育領域**: Chain-of-Thought Prompting 可以被用於教育領域，幫助學生更好地理解和解決複雜的問題。
* **研究領域**: 這項技術也可以被用於研究領域，幫助科學家更好地解決複雜的問題。

### Chain-of-Thought Prompting 的限制

* **模型的深度**: Chain-of-Thought Prompting 需要模型具有足夠的深度才能有效地工作。
* **模型的訓練資料**: 這項技術也需要模型被訓練在適合的資料上，才能有效地解決問題。

### 未來發展

* **進一步研究**: Chain-of-Thought Prompting 的研究仍然在進行中，未來可能會有更多的進展和應用。
* **實際應用**: 這項技術也將被用於實際的應用領域，例如教育、研究等。

**零槽方法 (Zero-Shot Approach)**
=====================================

### **問題描述**

*   問題: 如何在沒有示範例子的情況下使用零槽方法?
*   回答: 使用 "Let's think step by step" 的方法, 這樣可以讓模型自動產生推理步驟。

**相關概念**
------------

### **類比推理 (Analogical Reasoning)**

*   類比推理是指在沒有直接相關的例子的情況下, 使用類似的例子來解決問題。
*   這種方法可以幫助模型自動產生相關的方程式和策略。

**實驗結果**
-------------

### **競賽成績**

*   使用類比推理的方法在競賽中取得了出色的成績, 甚至超越了零槽方法。
*   這表明類比推理是一種有效的方法, 可以幫助模型自動產生相關的方程式和策略。

### **對 AGI 的影響**

*   這種方法可能有助於進一步了解人工智慧 (AGI) 的發展。
*   因為它可以幫助模型自動產生相關的方程式和策略, 這可能會使得 AGI 的開發更容易。

**Adaptive Example Generation**
=====================================

### Introduction

* Found related problems on the web
* Key idea: adaptively generate relevant examples and knowledge for each given problem
* Instead of using a big set of examples, like in manual chain-of-thought prompting

### Zero-Shot Reasoning

* Can use few-shot examples to show the model how to do step-by-step reasoning
* What can be done zero shot, without using any examples?
	+ Just see, let's think step by step
* Is it possible to trigger a step-by-step reasoning, even without using any prompt?

### Fine-Tuning and Chain-of-Thought Reasoning

* Models are fine-tuned or trained on many examples in the data mixture
* Recent work: "Chain-of-thought Reasoning without Prompting"
* Without prompting, means without seeing anything. Just give the problem to the model.

### Example Generation

* Decoding, in the first step, we look at all possible tokens
* Started with top-5 tokens and then continue greedy decoding
* First token is 5, and the next token was five apples
* If use top-2 tokens is I, then the fourth generation will be I have 3 apples...

### Reasoning without Prompting

* Model can do some reasoning if we started from different tokens
* Another example: Nicolas Cage born in even or odd year?
	+ First one say OK, Nicolas Cage was born in odd year.
	+ Second one says "even" and then period.
	+ Third one is "odd," period, OK?

### Conclusion

* How to find chain-of-thought reasoning without prompting?
	+ Take longer sentences
	+ Longer sentence means the model could do some reasoning steps.

**Chain-of-Thought Decoding**
=====================================

### Key Observations

*   Nicolas Cage was born in an odd year, and the probability is low.
*   However, if there's a reasoning path, like the last one, Cage was born in 1964, an even year.
*   The model is well-calibrated, with sentence probabilities jumping to 0.978.

### Pre-trained LLMs

*   Have had responses with step-by-step reasoning among generations started with top-k tokens.
*   Don't need to use prompts here.
*   Higher confidence in decoding the final answer on a step-by-step reasoning path is present.

### Comparison between Greedy Decoding and Chain-of-Thought Decoding

*   Chain-of-thought decoding performs much better than greedy decoding.

### Generating Intermediate Steps

*   Are helpful, but any concern on generating intermediate steps instead of direct answers?

### Concerns about LLMs

*   LLMs are probabilistic models of generating next tokens.
*   They are not humans and can make mistakes.
*   What we want is argmax, probability final answer given problem.

### Computing the Probability of Final Answer Given Problem

*   We should sum over all possible reasoning paths.
*   The total probability is computed from our course, what we learned.

**機器學習**
================

### **自我一致性**

*   **定義**: 自我一致性是指使用機器學習模型預測答案時，確保輸出的結果與原始問題的一致性。
*   **方法**: 使用多次樣本並選擇最常見的答案來實現自我一致性。

### **最大邊緣推斷**

*   **定義**: 最大邊緣推斷是指在預測答案時，考慮所有可能的結果並選擇最有可能的答案。
*   **方法**: 使用機器學習模型來計算每個答案的可能性，並選擇最大可能性值。

### **自由形式答案**

*   **定義**: 自由形式答案是指允許使用者輸入任何形式的答案，而不是限制在特定的選項中。
*   **方法**: 使用自我一致性和最大邊緣推斷來確保輸出的結果與原始問題的一致性。

### **實現**

*   **步驟 1**: 使用機器學習模型預測答案
*   **步驟 2**: 使用多次樣本並選擇最常見的答案來實現自我一致性
*   **步驟 3**: 使用最大邊緣推斷來確保輸出的結果與原始問題的一致性

### **優點**

*   **提高準確率**: 自我一致性和最大邊緣推斷可以幫助提高預測答案的準確率。
*   **簡化流程**: 使用自我一致性和最大邊緣推斷可以簡化預測答案的流程。

### **缺點**

*   **增加計算複雜度**: 自我一致性和最大邊緣推斷需要額外的計算資源來實現。
*   **可能出錯**: 如果使用者輸入的答案不符合原始問題，自我一致性和最大邊緣推斷可能會出錯。

**LLMs 的限制**
================

### 1. **Irrelevant Context**

*   Irrelevant information 可能會降低 LLMs 的問題解決能力。
*   試驗結果顯示，LMMs 在面對多餘資訊時可能會錯誤。

### 2. **無法自我糾正推理**

*   LLMs 無法自我糾正錯誤的推理。
*   即使提供提示，LLMs 也可能會錯誤。

### 3. **無法忽略多餘資訊**

*   提供提示 "ignore irrelevant context" 可能有助於 LLMS 忽略多餘資訊，但仍然存在問題。
*   如果多餘資訊過大，LLMs 的表現會下降。

### 4. **無法回收錯誤**

*   即使 LLMS 發現錯誤，也無法自我糾正。
*   提供提示 "Review your previous answer and find problems with your answer" 可能有助於 LLMS 回收錯誤，但仍然存在問題。

### 5. **LLMs 的限制**

*   LLMs 有多個限制，包括無法忽略多餘資訊、無法自我糾正推理和無法回收錯誤。
*   這些限制可能會影響 LLMS 的表現。

**自正確答案的問題**
=====================

### 自正確答案的方法

*   **錯誤答案**: [55:12] 自正確答案可能會改變正確答案為錯誤。
*   **無法改善**: [55:20] 我們進行了廣泛研究，包括 GSM8K、CommonSenseQA 和 HotpotQA 等基準測試，但沒有發現任何改善。

### 多個 LLMS 的辯論

*   **多個 LLMS 辯論**: [56:21] 使用多個 LLMS 進行辯論，直到達成一致或共識。
*   **無法超越自正確答案**: [57:09] 我們嘗試了這種方法，但發現它無法超越自正確答案。

### 自正確答案的缺點

*   **需要 oracle 反饒**: [57:21] 如果要使用自正確答案，則需要 oracle 反饒。
*   **oracle 反饒是必要的**: [57:29] 如果 oracle 反饒是必要的，那麼我們的工作就是自 debug。

### LLMS 的推理

*   **推理順序很重要**: [58:08] 在某些情況下，推理順序很重要。
*   **模型訓練資料**: [58:31] 模型被訓練於所有網路上的資料，因此可能會有順序問題。

### 測試 LLMS

*   **生成不同的評估任務**: [58:43] 生成不同的評估任務來測試 LLMS。
*   **重新排列句子**: [59:02] 重新排列原始 GSM8K 問題，看看模型是否仍然可以解決它。

**LLM (Large Language Model) 的研究**
=====================================

### 一、問題與挑戰

*   **中斷**: LLM 在解決問題時會遇到中斷，無法繼續推理。
*   **順序**: 重新排列問題的順序會對 LLM 的表現產生重大影響。

### 二、實驗設計

*   **實驗設計**: 設計合適的實驗來評估 LLM 的表現。
*   **中斷與順序**: 透過實驗設計，評估中斷和順序對 LLM 表現的影響。

### 三、結果與結論

*   **中斷與順序**: 結果顯示，中斷和順序會對 LLM 的表現產生重大影響。
*   **實驗設計**: 實驗設計是評估 LLM 表現的一個關鍵步驟。

### 四、未來工作

*   **挑戰**: 未來的挑戰在於定義一個合適的問題，並從第一原理出發解決它。
*   **AGI (Artificial General Intelligence)**: AGI 的研究需要進一步探索。

**機器學習**
================

### 重要概念

*   **語言模型**
*   **會議**

### 項目列表

#### 會議相關資訊

*   名稱: Conference on Language Modeling
*   主辦人: 多位優秀專家
*   目的: 瞄準語言模型領域

#### 其他資訊

*   時間: 未知
*   地點: 未知

---
## 參考資料
- 原始影片：[CS 194/294-196 (LLM Agents) - Lecture 1, Denny Zhou](https://youtube.com/watch?v=QL-FS_Zcmyo)
