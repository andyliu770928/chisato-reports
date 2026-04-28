# 【研究主題】AI名詞的基本介紹

- **研究日期：** 2026-04-28
- **研究範圍：** 人工智慧領域核心名詞的定義、層級關係與重要術語
- **研究深度：** 深度版
- **研究目的：** 系統性整理AI領域最常見的名詞，建立清晰的知識框架，便於快速理解與查閱

---

## 一、核心結論

### 1. 先講結論

- AI是最大的概念範疇，機器學習（ML）是AI的主要實現方式，深度學習（DL）則是ML的子領域，三者形成「AI ⊇ ML ⊇ DL」的包含關係。
- 大型語言模型（LLM）是NLP與深度學習融合的產物，也是2020年代生成式AI爆發的核心技術。
- Transformer架構（2017年）取代了傳統RNN/CNN，成為當代LLM的主流基礎。
- 理解AI名詞的關鍵在於掌握「從資料中學習」這條主線：監督式學習需要標籤、非監督式學習尋找結構、強化學習透過獎懲反饋優化策略。

### 2. 決策意義

- **這代表什麼：** 建立正確的名詞階層觀念，是理解任何AI文章、報告或投資標的的前提。
- **適合誰看：** 想快速掌握AI領域術語的初學者，或需要複習名詞的投資人與產品經理。
- **目前信心等級：** 高（主要基於Wikipedia公開知識，經多來源交叉比對）

---

## 二、研究問題與方法

### 1. 研究問題

1. AI、ML、DL三者的層級關係為何？
2. 機器學習三大範式（監督式、非監督式、強化學習）的核心差異？
3. Transformer為何重要？與傳統NN架構有何不同？
4. LLM與生成式AI的關係？
5. 常見訓練相關名詞（Epoch、Batch size、過擬合等）的意義？

### 2. 研究方法

- **第一輪：** 廣泛搜尋Wikipedia英文條目，擷取各核心名詞的intro段落，建立名詞清單與初步框架。
- **第二輪：** 針對Transformer、Embedding、RLHF、RAG等較複雜概念深入查閱，並補充層級關係與代表性論文。
- **來源類型：** Wikipedia（英文為主）、學術論文摘要、技術部落格共識。
- **排除原則：** 未具名來源的部落格文章、明星個人解讀、2020年前的過舊資料（ML/DL領域進步快速）。

---

## 三、研究筆記摘要

### 1. 關鍵數字

| 指標 | 數值 | 年份 | 來源 |
|------|------|------|------|
| AI一詞正式提出 | 1956年 | 1956 | Wikipedia (Dartmouth Conference) |
| 深度學習突破年 | 2012年 | 2012 | AlexNet論文 (Hinton et al.) |
| Transformer論文發布 | 2017年 | 2017 | Vaswani et al., "Attention Is All You Need" |
| RNN→Transformer轉換 | 2017年後 | 2017-2020 | 學界共識 |

### 2. 重要事件時間線

| 日期 | 事件 | 影響 | 來源 |
|------|------|------|------|
| 1956 | Dartmouth Conference，AI一詞正式誕生 | 確立AI為獨立研究領域 | Wikipedia |
| 1986 | Backpropagation演算法成熟 | 使訓練多層神經網路成為可能 | Rumelhart, Hinton & Williams論文 |
| 2012 | AlexNet以CNN赢得ImageNet競賽，深度學習復興 | 開啟深度學習黃金十年 | Krizhevsky et al. |
| 2017 | Transformer架構論文發表 | 奠定現代LLM與生成式AI的基礎 | Vaswani et al. (Google Brain) |
| 2020後 | GPT-3、ChatGPT相繼問世 | 生成式AI進入大眾市場 | OpenAI公告 |

### 3. 主要玩家 / 主要對象

| 名稱 | 角色定位 | 最新動態 | 觀察重點 | 來源 |
|------|----------|----------|----------|------|
| OpenAI | LLM與生成式AI領導者 | GPT-4o、o1/o3系列 | 技術領先程度與商業化 | openai.com |
| Google DeepMind | Transformer原創團隊 | Gemini系列 | 是否能追趕OpenAI | deepmind.google |
| Anthropic | AI安全與RLHF先驅 | Claude系列 | 對齊技術（Constitutional AI） | anthropic.com |
| Meta AI | 開源模型推動者 | Llama 3系列 | 開源vs封閉的產業影響 | meta.ai |
| 微軟 | AI應用與雲端整合 | Copilot全面嵌入產品線 | Azure AI營收成長 | microsoft.com |

---

## 四、主要發現

### 1. 發現一：AI的層級結構（AI ⊇ ML ⊇ DL）

AI是最大的概念，任何讓電腦具有人類智慧行為的技術都屬於AI。機器學習是AI的子領域，專注於讓系統從資料中自動學習規則，而非人工編寫固定邏輯。深度學習則是ML的子領域，使用多層神經網路（通常3層以上，實際可達數百至數千層）自動學習資料的階層式表徵。

這個層級關係非常重要：當媒體報導「AI突破」時，多數情況指的是深度學習的突破；當我們討論「LLM投資」時，底層是Transformer深度學習架構。理解層級可以避免把不同層次的技術混為一談。

### 2. 發現二：機器學習三大範式各有適用場景

**監督式學習（Supervised Learning）** 是最常見的方式。演算法根據「輸入-輸出配對」的標籤資料學習。例如：給定房屋坪數與成交價的資料，訓練後可預測新房屋的價格。優點是精準，缺點是需要大量已標籤資料。

**非監督式學習（Unsupervised Learning）** 在沒有標籤的資料中尋找結構，例如將客戶分群（ clustering）、降低資料維度（PCA）或學習資料的機率分布。適合探索性分析，但應用相對有限。

**強化學習（Reinforcement Learning）** 是讓智慧代理（agent）在環境中透過「動作-觀察-獎勵」循環自行學習最佳策略。2023年後的RLHF（Reinforcement Learning from Human Feedback）使LLM能根據人類偏好微調輸出品質，是ChatGPT等系統能對話流暢的關鍵技術之一。

### 3. 發現三：Transformer架構的突破性意義

在Transformer（2017）出現之前，NLP主要使用RNN（循環神經網路）處理序列資料，但RNN難以並行訓練且有梯度消失問題。Transformer以「注意力機制（Attention Mechanism）」取代了序列依賴，讓模型能同時关注序列中的所有位置，大幅提升訓練效率與表達能力。

Transformer的Self-Attention機制讓每個輸入token都能「注意」到序列中的其他token，捕捉長距離依賴關係。這是GPT、BERT等所有現代LLM的基礎。簡單來說：沒有Transformer，就沒有2020年代的LLM熱潮。

### 4. 發現四：生成式AI vs 判別式AI

**判別式AI（Discriminative AI）** 任務是對輸入資料進行分類或預測，例如：辨識照片中是否有貓、判斷郵件是否為垃圾郵件。傳統ML/DL模型多屬此類。

**生成式AI（Generative AI）** 則是學習資料分布，進而生成新資料（如文字、圖像、音頻、程式碼）。GAN（生成對抗網路，2014）和Diffusion Model（2020年代）是圖像生成的兩大主流技術。LLM則是文字生成的代表。兩者的核心差異在於：判別式回答「這是什麼」，生成式回答「這可以產生什麼」。

### 5. 發現五：LLM、生態系統與周邊技術

**Token** 是LLM處理文字的基本單位，可以是一個詞、子詞（subword）或字元。LLM輸出的流暢度與tokenize方式高度相關。

**Embedding（嵌入）** 將高維度資料（如文字、圖像）映射到低維度向量空間，使語意相似的內容在向量空間中距離接近。這是NLP所有深度學習模型的基礎技術。

**Prompt Engineering（提示工程）** 是設計輸入提示以引導LLM產生更準確輸出的技術，包括Few-shot prompting、Chain-of-Thought等技巧。

**RAG（Retrieval-Augmented Generation）** 讓LLM在回答前先從外部資料庫抓取相關資訊，緩解LLM知識過時與幻覺（Hallucination）問題。

**Fine-tuning（微調）** 是在已預訓練的模型基礎上，用特定任務資料進一步訓練，使模型適應特定領域或任務。

---

## 五、矛盾點與不確定性

### 1. 來源之間的矛盾

| 爭議點 | 來源A | 來源B | 我的判讀 |
|--------|-------|-------|----------|
| AGI時間表 | 部分專家認為10-20年內 | 多數研究者認為仍需數十年 | 短期內（2026）AGI到來的機率低，投資人不應過度期待 |
| 深度學習是否已觸瓶頸 | LeCun等認為規模化仍有空間 | 部分研究者認為Transformer红利已盡 | 規模化瓶頸已顯，但新架構（MoE、State Space）仍在推進 |

### 2. 目前仍未補齊的資訊

- 各名詞的數學推導細節（如Attention的矩陣運算細節）
- 各名詞的台灣產業應用實例
- CNN/RNN/Transformer三者的詳細技術比較表格
- 各名詞的代表性論文完整清單

### 3. 可能造成誤判的風險

- 過度簡化：將所有AI進展都歸功於「LLM」，忽略傳統ML在特定領域（推薦系統、金融風控）的持續重要性。
- 術語混淆：媒體常將「AI聊天機器人」與「真正的AI」混為一談，影響判斷。
- 過擬合心態：以為學會名詞就等於理解技術，兩者差距仍大。

---

## 六、情境分析

### 1. 基準情境

- **假設：** AI技術持續按照目前軌跡演進，Transformer生態系繼續擴大。
- **可能結果：** LLM在各產業滲透率持續提升，但通用AGI仍遙遠。
- **觀察指標：** OpenAI/Anthropic/Google模型更新頻率、LLM相關資本支出。

### 2. 樂觀情境

- **假設：** 新架構突破（如更高效Transformer、新的Attention變體）使AI能力階梯式提升。
- **可能結果：** AI取代白領重複性工作的速度超預期。
- **觀察指標：** 論文發布品質、模型Benchmark突破訊號。

### 3. 保守情境

- **假設：** LLM規模化遇到能源/算力瓶頸，新模型進展放緩。
- **可能結果：** AI投資熱潮退燒，資金重新聚焦於有明確ROI的特定ML應用。
- **觀察指標：** GPU供應鏈財報、NVIDIA營收成長率、數據中心用電量。

---

## 七、對 Andy 的實際建議

### 1. 如果你是要快速理解

記住一個框架：**AI > ML > DL > LLM/生成式AI**。見到任何AI名詞，先問它在這個金字塔的哪一層。

### 2. 如果你是要做決策

- **優先關注：** LLM與生成式AI的商業化進展（RAG應用、微調模型、Agent系統）。
- **暫時不要過度解讀：** AGI相關言論與時間表預測，多數不靠譜。
- **下一步建議：** 若要深入特定AI投資主題（如：AI基礎建設、ML系統整合、AI應用軟體），建議先從該主題的代表性公司營收與產品進展切入，而非糾結於底層技術名詞。

### 3. 後續追蹤清單

1. 追蹤Transformer後新架構（如Mamba、State Space Model）的進展。
2. 追蹤RLHF與AI對齊技術的實際產品影響（Claude vs GPT能力差異）。
3. 追蹤RAG與Fine-tuning在企業端實際部署的情況。

---

## 八、資料來源

### 1. 核心來源

1. Wikipedia - Artificial intelligence｜n.d.｜https://en.wikipedia.org/wiki/Artificial_intelligence
2. Wikipedia - Machine learning｜n.d.｜https://en.wikipedia.org/wiki/Machine_learning
3. Wikipedia - Deep learning｜n.d.｜https://en.wikipedia.org/wiki/Deep_learning
4. Wikipedia - Large language model｜n.d.｜https://en.wikipedia.org/wiki/Large_language_model
5. Wikipedia - Transformer (deep learning model)｜n.d.｜https://en.wikipedia.org/wiki/Transformer_(deep_learning_model)
6. Vaswani et al. - "Attention Is All You Need"｜2017｜https://arxiv.org/abs/1706.03762
7. Wikipedia - Generative artificial intelligence｜n.d.｜https://en.wikipedia.org/wiki/Generative_artificial_intelligence
8. Wikipedia - Reinforcement learning｜n.d.｜https://en.wikipedia.org/wiki/Reinforcement_learning

### 2. 輔助來源

1. Wikipedia - Supervised learning｜n.d.｜https://en.wikipedia.org/wiki/Supervised_learning
2. Wikipedia - Unsupervised learning｜n.d.｜https://en.wikipedia.org/wiki/Unsupervised_learning
3. Wikipedia - Retrieval-augmented generation｜n.d.｜https://en.wikipedia.org/wiki/Retrieval-augmented_generation
4. Wikipedia - Fine-tuning (deep learning)｜n.d.｜https://en.wikipedia.org/wiki/Fine-tuning_(deep_learning)
5. Wikipedia - Reinforcement learning from human feedback｜n.d.｜https://en.wikipedia.org/wiki/Reinforcement_learning_from_human_feedback
6. Wikipedia - Hallucination (artificial intelligence)｜n.d.｜https://en.wikipedia.org/wiki/Hallucination_(artificial_intelligence)
7. Wikipedia - Embedding (machine learning)｜n.d.｜https://en.wikipedia.org/wiki/Embedding_(machine_learning)
8. Wikipedia - Prompt engineering｜n.d.｜https://en.wikipedia.org/wiki/Prompt_engineering

---

## 九、附錄

### 1. 名詞對照表（英文↔繁體中文）

| 英文 | 中文 | 所屬層級 |
|------|------|----------|
| Artificial Intelligence (AI) | 人工智慧 | 頂層 |
| Machine Learning (ML) | 機器學習 | 第二層 |
| Deep Learning (DL) | 深度學習 | 第三層 |
| Neural Network (NN) | 神經網路 | 技術基礎 |
| Artificial Neural Network (ANN) | 人工神經網路 | 同上 |
| Supervised Learning | 監督式學習 | ML範式 |
| Unsupervised Learning | 非監督式學習 | ML範式 |
| Reinforcement Learning (RL) | 強化學習 | ML範式 |
| Natural Language Processing (NLP) | 自然語言處理 | AI應用領域 |
| Large Language Model (LLM) | 大型語言模型 | NLP+DL產物 |
| Generative AI (GenAI) | 生成式人工智慧 | AI應用領域 |
| Transformer | Transformer模型 | DL架構 |
| Attention Mechanism | 注意力機制 | 核心技術 |
| Self-Attention | 自注意力機制 | Transformer核心 |
| Convolutional Neural Network (CNN) | 卷積神經網路 | DL架構 |
| Recurrent Neural Network (RNN) | 循環神經網路 | DL架構（已過渡） |
| Generative Adversarial Network (GAN) | 生成對抗網路 | 生成模型 |
| Diffusion Model | 擴散模型 | 生成模型 |
| Backpropagation | 反向傳播 | 訓練演算法 |
| Gradient Descent | 梯度下降 | 優化演算法 |
| Loss Function | 損失函數 | 訓練目標 |
| Overfitting | 過擬合 | 訓練問題 |
| Underfitting | 欠擬合 | 訓練問題 |
| Hyperparameter | 超參數 | 訓練設定 |
| Token | Token/詞元 | LLM基本單位 |
| Embedding | 嵌入/向量嵌入 | 表徵學習 |
| Prompt Engineering | 提示工程 | LLM互動技術 |
| Fine-tuning | 微調 | 模型訓練技術 |
| Transfer Learning | 遷移學習 | 訓練策略 |
| Retrieval-Augmented Generation (RAG) | 檢索增強生成 | LLM擴展技術 |
| Reinforcement Learning from Human Feedback (RLHF) | 人類回饋強化學習 | 對齊技術 |
| Hallucination | 幻覺/錯覺（AI） | LLM問題 |
| Epoch | 訓練輪次 | 訓練設定 |
| Batch Size | 批次大小 | 訓練設定 |
| Training/Validation/Test Set | 訓練/驗證/測試集 | 資料划分 |
| Artificial General Intelligence (AGI) | 通用人工智慧 | 假設型AI |
| Narrow AI / Weak AI | 弱人工智慧/狹義AI | 當前主流 |
| Computer Vision | 電腦視覺 | AI應用領域 |
| Speech Recognition | 語音辨識 | AI應用領域 |
| Word Embedding | 詞嵌入 | NLP技術 |
| Feature Engineering | 特徵工程 | ML前處理 |
| Activation Function | 啟動函數 | 神經網路元件 |

---

*本報告使用兩階段研究流程整理，重點在可追溯、可驗證、可延伸。*
