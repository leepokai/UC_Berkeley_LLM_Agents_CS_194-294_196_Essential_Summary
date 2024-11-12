# CS 194/294-196 (LLM Agents) - Lecture 8, Yuandong Tian

## 課程筆記

**Yuandong Tian 的演講筆記**
=====================================

### 簡介
-----------------

* 名字: Yuandong Tian
* 職位: Meta AI FAIR 研究科學家指導者

### 主題
--------------

* **統一框架**: Neural 和 Symbolic 決策的統一框架

### 說明
-------------

#### 介紹
----------------

* 說明演講主題: Reasoning 和 Planning Domain 的研究

#### 應用場景
----------------

* 列出語言模型在不同應用場景中的使用情況:
	+ 口述 AI
	+ 內容生成
	+ 角色扮演
	+ AI 代理人
	+ Reasoning 和 Planning

#### 問題
--------------

* 說明語言模型在 Reasoning 和 Planning Domain 中的問題:
	+ 行動模型的缺陷

### 旅行規劃問題
-------------------

* 描述旅行規劃問題:
	+ 要求生成一個可執行、可行和最佳的行程

### 解決方案
--------------

* 提出解決方案:
	+ 使用語言模型來查詢資訊
	+ 進行身份行為
	+ 利用統一框架來強化 Reasoning 和 Planning 能力

**旅行規劃**
================

### 介紹
----------------

*   **外部資訊**: 從外部世界取得大量資訊
*   **語言模型**: 問題語言模型進行搜尋、航班查詢和酒店查詢等任務

### 旅行規劃流程
-------------------

1.  **搜尋與查詢**:
    *   問語言模型進行搜尋、航班查詢和酒店查詢等任務
    *   取得多個可能的目的地、航班資訊和酒店資訊
2.  **整合資訊**:
    *   將取得的資訊整合在一起
3.  **規劃**:
    *   使用語言模型進行旅行規劃
    *   根據取得的資訊建立一份可執行的行程

### 問題與挑戰
-----------------

*   **旅行規劃任務**: 使用語言模型進行旅行規劃時遇到的問題和挑戰
*   **結果**:
    *   即使使用 GPT-4 Turbo 進行旅行規劃，最終通過率也只有 0.6% 和 4.4%
    *   表明語言模型在這類任務中仍有很大的改進空間

### 結論
----------

*   **旅行規劃**: 一個複雜的任務需要結合多個資訊源和使用語言模型進行規劃
*   **挑戰**:
    *   使用語言模型進行旅行規劃時遇到的問題和挑戰

**旅行規劃問題**
================

### 問題描述

*   旅行規劃問題的效率不佳，尤其是在複雜度增加時。
*   Gemini 模型在這些基準中表現良好，但在更複雜的案例中表現不佳。

### 解決方案類別

1.  **Scaling Law**
    *   這是一種解決方案，能夠有效地處理複雜度增加的情況。
2.  **Fine-tuning**
    *   這是另一種解決方案，通過微調模型來提高效率。
3.  **Hybrid Approach**
    *   這是第三種解決方案，結合了Scaling Law和Fine-tuning的優點。

### 結論

*   旅行規劃問題仍然是一個挑戰性的問題。
*   需要進一步研究和開發有效的解決方案。

**深度學習與解決方案**
========================

### 選項一:使用更多數據、更強的計算能力和更大的模型

* 使用更多數據和更強的計算能力來改善性能
* 可能最終解決所有問題，但需要大量資源和工程挑戰
* 這是一種選擇，可能不是最好的選擇

### 選項二:混合系統

* 混合深度模型和符號求解器
* 深度模型優於自然語言理解，但不善於規劃任務
* 符號求解器可提供最佳解決方案，但無法理解自然語言
* 可能結合兩者來達到更強大的系統

### 選項三:符號表示的自動產生

* 使用深度學習來找到符號表示的自動產生方法
* 這是一種新興的研究領域，可能具有很大潛力

### 結合深度模型和符號求解器的方法

* 工具使用：結合深度模型和混合整數線性計畫（MILP）來改善性能
* 符號表示的自動產生：使用深度學習來找到符號表示的自動產生方法

**ming 和 Neural Network**
==========================

### **問題描述**

*   使用更大型的模型來解決旅行規劃問題
*   將自然語言輸入轉換為 JSON 檔案
*   利用混合整數線性計畫 (MILP) 決策器求出最佳行程

### **解決方案**

#### **步驟 1: 轉換自然語言輸入**

*   使用語言模型將自然語言輸入轉換為 JSON 檔案
*   JSON 檔案包含使用者要求的符號表示

#### **步驟 2: 利用 MILP 決策器**

*   將 JSON 檔案與航班和酒店資訊結合
*   使用 MILP 決策器求出最佳行程

#### **步驟 3: 回傳結果**

*   取得最佳行程的符號描述
*   轉換為實際句子回傳給使用者

### **實驗結果**

*   人類評估顯示系統有效且滿足使用者需求
*   系統相比基線有所改善

**對話式旅遊計畫**
=====================

### 背景
----------------

* 人們通常不會直接提供 JSON 檔案給旅行社
* 旅行社會先問一些基本問題，然後再進一步詢問細節

### 旅行社的需求
-------------------

* 需要能夠有效地取得旅客資訊
* 需要能夠在短時間內取得所有必要資訊
* 需要能夠適應不同類型的旅客行為

### 旅行社的目標
------------------

* 能夠有效地取得旅客資訊
* 能夠在短時間內取得所有必要資訊
* 能夠適應不同類型的旅客行為
* 能夠提供可靠和一致性的服務

### 旅行社的策略
-------------------

* 設計一個叫做 APEC 的代理人憲法
* 這個憲法包含四個部分：
	+ 精確性：代理人需要能夠準確地取得資訊
	+ 主動性：代理人需要能夠主動地詢問旅客
	+ 效率：代理人需要能夠在短時間內取得所有必要資訊
	+ 可靠性：代理人需要能夠提供可靠和一致性的服務

### 測試與評估
-----------------

* 設計 50 個不同的旅客行為
* 每個行為都會有私人的隱藏表格，包含最重要的資訊
* 這些行為需要能夠在短時間內取得所有必要資訊
* 測試結果將用於評估代理人性能

**深度模型與求解器的整合**
=====================================

### 第一部分: 使用深度模型來評估求解器

*   **Overall**: 指的是所有入口。
*   **Critical**: 指的是對特定人物的重要入口。
*   **Persona**: 指的是旅行者的個性或角色。
*   **Agent Constitution**: 指的是使用求解器作為評判者來改善性能的方法。

### 第二部分: 將求解器與深度模型結合

*   **Search Former Results**: 指的是使用求解器提供的資料來訓練更好的深度模型。
*   **Planning Task**: 指的是規劃任務，例如在迷宮中找到最短路徑。

### 第三部分: 使用求解器作為評判者

*   **Agent as Judge**: 指的是使用求解器作為評判者來評估其他求解者的行為。
*   **Feedbacks**: 指的是提供給求解者的反饋資訊，以幫助其改善。

### 第四部分: 結合求解器與深度模型的研究方向

*   **Combining Agent and Deep Models**: 指的是結合求解器和深度模型來完成任務。
*   **Research Directions**: 指的是探索使用求解器提供資料來訓練更好的深度模型的可能性。

**A\* Search**
===============

### 什麼是 A\* Search

*   **定義**: A\* Search 是一個用於找到最短路徑的演算法。
*   **特點**: 它使用 heuristic function 來估計未知路徑的成本。

### A\* Search 的運作流程

1.  **創建新節點**: A\* Search 創建新的節點並探索不同部分的迷宮，以找到能夠到達目的地的路徑。
2.  **創建中間步驟**: 這個過程會創建中間步驟，顯示如何到達最優解。

### 搜索增強模型

*   **定義**: 搜索增強模型是一種模型，它使用 A\* Search 的結果來預測最終的最佳方案。
*   **特點**: 它能夠創建更長的 token 序列，因為它會輸出搜索過程和最優解。

### 相關概念

*   **符號求解器**: 符號求解器是一種用於找到最短路徑的演算法。
*   **最佳方案預測**: 最佳方案預測是指使用 A\* Search 的結果來預測最終的最佳方案。

**Search Augmented Models**
==========================

### 什麼是 Search Augmented Models?

*   **定義**: Search Augmented Models 是一個可以用在許多不同情況下的模型。
*   **特點**: 這個模型的曲線不是非常完美。

### Search Augmented Models 的優點

*   **效率**: 使用 Search Augmented Models 可以達到更高的性能，且只需要 50k 個樣本就可以達到 80% 的最終分數。
*   **參數效率**: Search Augmented Models 可以使用 10 倍少的參數來達到相同的性能。
*   **資料效率**: Search Augmented Models 可以使用 10 倍少的樣本來達到相同的性能。

### Search Augmented Models 的應用

*   **迷宮導航**: Search Augmented Models 可以用在迷宮導航中，例如 Sokoban 游戲。
*   **其他情況**: Search Augmented Models 可以用在許多不同的情況下。

### 未來的發展方向

*   **超越 Search Augmented Models**: Search Augmented Models 的效率和資料效率可以進一步改善。

**Beyond A\***
================

### **arch trace**

*   [27:58] 使用 search trace 訓練模型
*   [28:00] Transformer 會教導強迫模型來獲得 Search Augmented Model
*   [28:02] 這個模型已經是資料高效和時間高效的

### **search-augmented model**

*   [28:04] 使用 search-augmented models 進行 fine-tuning 以達到更短的 trace 但仍能導致最佳結果
*   [28:09] 這是一個典型的強化學習任務，最終得到 Search Former Model

### **expert activation**

*   [28:41] 不是真正的強化學習任務，而是 expert activation
*   [28:44] 只要做的是樣本多次並且具有多樣性
*   [28:49] 這樣的樣本會導致許多不同的選擇和結果
*   [28:53] 選擇最佳結果，並根據最佳結果檢查相關搜索詞

### **bootstrapping**

*   [28:16] 使用最佳結果建立訓練集並重新訓練模型
*   [28:19] 這個過程可以重複進行
*   [28:21] 每次都會得到更短的 trace 但仍能導致最佳結果

### **結果**

*   [29:27] 對比起來，相同或是更好的最佳率
*   [29:31] 但是分布的平均序列長度會變得越來越短
*   [30:23] 這個過程可以重複進行並且得到更好的結果

### **ILR**

*   [30:47] 定義一個 ILR 指標來衡量改善的長度比率

**A Star Search**
================

### **Length Ratio of Optimal Solution**

*   **Definition**: The ratio of the optimal solution to the trace discovered by neural networks.
*   **Improvement Over Time**: The length ratio improves over time, indicating that the final trace output by neural networks becomes shorter and more efficient.

### **Optimality Rate**

*   **Definition**: The rate at which the optimal solution is achieved.
*   **Improvement Over Time**: The optimality rate increases over time, indicating that the search former performance improves with each iteration of bootstrapping.

### **DualFormer**

*   **Introduction**: A follow-up paper to Search Former, introducing a V2 version of the algorithm.
*   **Weakness of Search Former**: The trace output by Search Former is often very long, taking thousands of tokens before giving the final outcome.
*   **Solution in DualFormer**: DualFormer reduces the length of the search trace by dropping randomly some portion of it. Different levels of dropping are defined, including:
    *   Dropping close costs in A star search
    *   Dropping cost tokens in create center and clause
    *   Dropping entire query costs
    *   Level 4: Dropping the entire trace and using solution-only data to train models

**Dual Former**
================

### **Introduction**

*   **Diversity**: 定義為生成的 rollout 數量與 cluster 數量之比（64）
*   **高多樣性**：對於測試時間計算而言，重要，因為它能夠改善性能
*   **Dual Former**：一個簡單的方法，可以自動給出高多樣性的結果

### **實驗結果**

*   **訓練模型**: 將所有不同層級的追蹤組合起來，然後進行訓練
*   **結果**: 表現比只使用解決方案或完整追蹤的兩種情況都好
*   **測試**: 在迷宮大小不同的環境中進行測試，並且在全局任務上取得了更好的表現

### **Dual Former 的特點**

*   **自動切換模式**：根據問題規格，能夠自動切換為快速模式或慢速模式
*   **適應性**: 對於不同的模型都能夠工作良好

### **系統 1 和系統 2**

*   **系統 1**: 直接預測最終解決方案
*   **系統 2**: 先進行搜索過程，然後給出最終解決方案

### **Dual Former 的驚人行為**

*   **自動切換**：訓練在混合資料上的模型，可以自動切換為系統 1 和系統 2
*   **輸出結果**：能夠直接給出答案或進行慢速思考過程，然後給出最終解決方案

**深度學習模型**
================

### **雙前者模式**

*   **定義**: 雙前者模式是一種訓練模型的方法，讓它能夠產生不同類型的輸出。
*   **特點**: 
    *   可以控制前者的運作方式
    *   可以控制輸出的第一個token
    *   可以在快速和慢速模式之間切換

### **實驗結果**

*   **雙前者模型**:
    *   在系統1和系統2的基礎上訓練出來的模型，能夠達到比單獨訓練在系統1或系統2上的模型更好的表現
    *   可以控制前者的運作方式，從而影響輸出的類型
*   **快速模式**:
    *   強迫前者使用快速模式，能夠產生比基礎模型更好的表現
*   **慢速模式**:
    *   強迫前者使用慢速模式，能夠產生比基礎模型更好的表現

### **數學問題**

*   **AugMATH資料集**:
    *   有一個很長的解釋，描述了如何得到答案
    *   可以隨機刪除句子，訓練出來的模型能夠產生比基礎模型更好的表現

### **結論**

*   雙前者模式是一種有效的方法，可以讓模型在快速和慢速模式之間切換
*   這種方法可以用於不同的應用場景，例如系統1和系統2的基礎上訓練出來的模型。

**AugMATH**
================

### 第一部分：比較與分析

#### 比較與結果

*   **Dual Form vs 原始數據集**: AugMATH 的 Dual Form 在性能上比原始數據集更好，且在 trace length 上也更短。
*   **Dual Form 的優勢**:
    *   能夠給出正確的路徑和出口狀態
    *   能夠做到良好的規劃和合理的結果

#### 比較與限制

*   **比較基準**: 這個比較不是完全公平，因為原始數據集應該有精煉過的版本。

### 第二部分：訓練模型

#### 訓練方法

*   **結合 Combinatorial Solver 和 Model Training**:
    *   使用 Combinatorial Solver 解決複雜的問題
    *   進行端到端的訓練，同時對模型和解決方案進行改進

### 第三部分：應用與範例

#### 例子：桌面佈置

*   **桌面佈置**: 將 k 個桌面分配到相同的設備上，以便每個設備都能夠承擔大量桌面的計算，同時避免超出記憶體容量。
*   **目標**: 最小化延遲時間。

**Neural Network Optimization**
=====================================

### 問題描述
-----------------

*   **問題**: 將表格 I 放置在裝置 J 上的最佳方法。
*   **變數**: x (二進位變數) 代表表格 I 是否被放置在裝置 J 上。

### 適用程式
----------------

#### 限制條件
-----------------

1.  **每個表格 I**：該表格應該與某個裝置 J 放置。
2.  **每個裝置 J**：最終記憶體消耗不應超過任何記憶體預算。

### 適用程式
----------------

#### 限制條件
-----------------

1.  **每個表格 I**：該表格應該與某個裝置 J 放置。
2.  **每個裝置 J**：最終記憶體消耗不超過 MJ。

### 結果
----------

*   **問題**: 將表格 I 放置在裝置 J 上的最佳方法。
*   **變數**: x (二進位變數) 代表表格 I 是否被放置在裝置 J 上。

### 適用程式
----------------

#### 線性問題
-----------------

1.  **輸入**: 問題描述 y。
2.  **預測**: surrogat cost C。
3.  **解決方案**: 線性問題 x\*。

### 結果
----------

*   **最佳方法**: 將表格 I 放置在裝置 J 上的最佳方法。
*   **變數**: x (二進位變數) 代表表格 I 是否被放置在裝置 J 上。

**回歸係數 C**
================

### 回歸係數 C 的計算

*   [46:29] 回歸係數 C 將被插入求解器。
*   [46:32] 求解器將給出解。
*   [46:34] 這個解將被插入目標中，得到損失函數。

### 最佳化回歸係數 C

*   [46:43] 我們可以使用反向傳播來找到最佳化的回歸係數 C。
*   [46:51] 我們的目標是找到最小化損失的方法。
*   [47:09] 我們想要找到最佳化的回歸係數 C 的方式。

### 結果

*   [47:25] 這些想法在嵌入表格碎片中試驗成功。
*   [47:38] 左圖顯示解質量。
*   [47:41] 我們想要解的損失最小化。
*   [47:49] 理想情況下，損失為零。

### 部署時間

*   [47:53] 右圖也關注部署時間。
*   [47:59] 我們不希望部署過慢。
*   [48:02] 這時我們可以使用多種方法來減少部署時間。

### 多種方法

*   [48:08] 我們有三種變體：
    *   [48:11] 圈 0：在測試時間進行反向傳播，速度慢，但解質量好。
    *   [48:22] 圈前期：直接學習 C = Cy 映射，並使用映射預測 C 和呼叫求解器一次。
    *   [48:36] 混合版本：先用前期模組找到 C 的初始值，然後持續優化 C。

### 結果

*   [48:51] 我們的三種變體提供了良好的平衡，既能減少解損失，又能降低部署時間。
*   [49:01] 這包括現有的方法，如 DOMESTIC、HEURISTIC、GREEDY 和 DREAM SHOT 等。
*   [49:05] DREAM SHOT 使用強化學習來優化非線性最佳化問題。

**Inverse Photonic Design**
==========================

### **問題描述**

*   這是一個設計問題，目的是將光線從上面傳遞到下面的不同區域，依據其波長。
*   使用的技術是干涉和衍射，而不是鏡子，因為設計面積太小。

### **優點**

*   只需要預測一次係數C，就能得到最佳結果。
*   這個方法比傳統方法快很多，而且性能也很好。

### **其他應用**

*   這種方法也可以用在其他設計問題上，例如逆向光子設計。

### **逆向光子設計**

#### **描述**

*   這是一個80x80的超小型格網。
*   目標是將光線從上面傳遞到下面的不同區域，依據其波長。

#### **原理**

*   當光線通過這個格網時，它會像波動一樣行進，並在不同的位置干涉和衍射。
*   這使得光線能夠傳遞到下面的不同區域，依據其波長。

#### **限制**

*   由於設計面積太小，因此不能使用鏡子來實現這個效果。
*   必須使用干涉和衍射的原理來達成這個效果。

### **最佳化問題**

#### **描述**

*   這是一個複雜的最佳化問題，需要計算頻率響應、截止頻率等參數。
*   需要進行模擬以找到最佳設計方案。

#### **限制**

*   由於設計面積太小，因此必須使用brush來實現這個效果。
*   brush的大小成為了一個限制因素。

#### **非製造性問題**

*   如果有一個孤立的點出現在設計中，則該點將無法製造。
*   這使得最佳化問題更加複雜。

**左側的東西**
================

### **光學器件**

*   [52:30] 使用這種很好的 **aligner patterns**。
*   [52:33] 可以將光分成兩個不同的流。
*   [52:38] 這被稱為 **beam splitter**。
*   [52:40] 也可以做其他的工作，例如 **wavelength multiplier**。

### **設計優化**

*   [52:46] 我們正在使用我們的方法。
*   [52:50] 我們能夠找到一個好的設計使用這種優化技術。
*   [52:53] 這個曲線基本上表明了我們的方法叫做 **circle zero** 和 **circle hybrid**，有著一個更平滑的收斂曲線相比於現有的方法，稱為 **pass-through**。

### **限制**

*   [53:20] 有一些限制。
*   [53:25] 如果函數 f 不可微分，我們該怎麼做？
*   [53:30] 在訓練過程中，我們也需要呼叫解析器，每次都很慢。
*   [53:37] 還有其他的需求，例如 **[INAUDIBLE]**。

### **後續工作**

*   [53:45] 我們已經有一些後續工作來克服這些問題。
*   [53:51] 由於時間限制，我們不能詳細說明，但如果你感興趣，可以聯繫我們。
*   [53:56] 可以閱讀相關的論文和查看代碼。

### **結合系統**

*   [54:02] 這是第二部分的結束，主要介紹了 **hybrid systems**，這些系統可以使用神經網路和解析器。
*   [54:06] 在最後一部分，我們將討論第三個選項，即 **是否模型能夠收斂到符號上**。

### **符號收斂**

*   [54:20] 這是一個很有趣的問題，因為我們知道在 Twitter 或 X 上，有兩種不同的看法。
*   [54:33] 一部分人認為，當模型參數越來越大時，它們可以做到一切。
*   [54:41] 但另一部分人認為，這些模型可能不會做出什麼真正有智慧的行為。

**自然語言模型的理解**
=====================================

### 問題描述

*   **訓練集中的好例子**: 模型在訓練集中已經看到過好的例子，這使得它能夠做得相當不錯。
*   **Apple 的研究**: Apple 有一篇名為 "The [INAUDIBLE] Symbolic" 的論文，該論文展示了通過添加無關的主題和句子到 GSM 資料集中，模型在測試集中會出現巨大的性能下降。

### 問題分析

*   **模組加法**: 模型被要求進行模組加法，這是一個簡單的讀取任務。
*   **表達式理解**: 但是，當我們嘗試了解模型所學習到的表示時，我們發現它並不是一個完美的基礎。

### 解決方案

*   **兩層網絡**: 我們使用兩層網絡來分析和理解模型所學習到的表示。
*   **底層和頂層**: 我們將模型分成底層和頂層，底層負責處理輸入 A 和 B，而頂層則負責產生輸出 C。

### 結論

*   **表達式理解**: 透過分析兩層網絡的行為，我們可以更好地了解模型所學習到的表示。
*   **自然語言模型的挑戰**: 這個問題是自然語言模型的一個核心挑戰，需要深入研究和理解。

**Hidden Nodes and Fourier Transform**
=====================================

### Introduction

* Hidden nodes are used in neural networks to process information.
* They add together and send their activations to the top layer.

### Quadratic Activations

* Each hidden node uses quadratic activation functions.
* These activations will be sent to the top layer for further processing.

### Output Representation

* The output representation is compared with a 100-dimensional representation of C.
* This comparison is used to evaluate the performance of the neural network.

### Fourier Domain Analysis

* Converting everything to the Fourier domain makes it easier to analyze.
* The Fourier transform is used to get complex number coefficients Za, Zb, and Zc.

### Gradient Descent Solution

* The gradient descent solution shows a regular pattern.
* The x-axis represents hidden node index, and the y-axis represents frequency of the Fourier transform.

### Structure of Hidden Neurons

* For each frequency k, there are a few hidden neurons that show strong frequencies at that particular frequency k.
* The number of neurons showing strong correspondence for each frequency is interestingly structured.

### Statistics on Gradient Descent Solutions

* Checking more statistics on gradient descent solutions shows:
	+ Distribution of orders at different frequencies
	+ Training curves for D equals 23

**重要概念**
* **Semiring structure**: A mathematical structure that combines addition and multiplication operations.
* **Ring homomorphism**: A function that preserves the ring's addition and multiplication operations.

**筆記內容**

### 1. 數學結構
#### * Semiring Structure *

*   定義：一個具有加法和乘法運算的數學結構。
*   特點：在這個結構中，乘法是 Kronecker 產品，而加法是連接兩個隱藏神經元。

### 2. 數學概念
#### * Ring Homomorphism *

*   定義：一個函數，如果它能夠保留環的加法和乘法運算，那麼它就是環同態。
*   特點：這種函數能夠將部分解延伸到全局解。

### 3. 數學應用
#### * 解決方案 *

*   **重寫 MSE Loss**: 將 MSE Loss 重寫為一個新的形式，包含紅色、藍色和綠色的項。
*   **求解全局解**: 利用環同態的性質來求解全局解。

### 4. 數學推理
#### * 結論 *

*   **結合數學結構和概念**: 將 semiring structure 和 ring homomorphism 結合起來，得到一個新的數學框架。
*   **應用於神經網路**: 這個新框架可以用於分析和解決神經網路中的問題。

**Partial Solution**
=====================

### Concept

* **Ring Structure**: A mathematical structure that allows for multiplication and addition of partial solutions.
* **Global Optimization**: The process of finding the optimal solution to a problem by combining partial solutions.

### Key Points

#### Partial Solutions

* Z1 and Z2 are partial solutions that only satisfy one single term of the loss function.
* They are part solutions, not the entire solution.

#### Ring Structure

* Multiplying two partial solutions together results in a new solution that satisfies both constraints at the same time.
* This allows for gradual construction of more complicated solutions through multiplication and addition.

### Implications

* No need for gradient descent to find global optimal solutions.
* Solutions can be constructed algebraically, resulting in global optimal solutions to the original loss functions.
* Can construct solutions like order 6 by multiplying all three and two solutions together and adding over all possible frequencies.

### Real-World Connection

* The process is symbolic and abstract, but has an exact match with gradient descent solutions in certain settings.
* 95% of solutions can be factorized into either 2 by 3 or 2 by 2, which is the same as the construction done previously.
* 98% of solutions can be factorizable into the constructive forms.

**Descent Solution Matches**
==========================

### 概念介紹

* **_Neural Network_**: 人工神經網路
* **_Gradient Descent_**: 梯度下降演算法
* **_Symbolic Representation_**: 符號表示法

### 結果與意義

#### 1. 符號表示法的出現

* 在某些情況下，人工神經網路可以產生符號表示法的解決方案
* 這可能是未來研究的一個方向

#### 2. 替代梯度下降演算法

* 人工神經網路可以提供替代的方法來求解問題
* 這可能會減少梯度下降演算法的使用

### 未來展望

* 可能不再需要梯度下降演算法
* 代之的是幾何構造來組合小解決方案成大解決方案

---
## 參考資料
- 原始影片：[CS 194/294-196 (LLM Agents) - Lecture 8, Yuandong Tian](https://youtube.com/watch?v=wm9-7VBpdEo)
