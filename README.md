# popmart_douyin_comment_analysis
This project analyzes user comments from Douyin regarding Pop Mart products. The goal is to clean the text data, perform sentiment analysis to focus on positive feedback, and then extract key adjectives to identify prevalent flat design style keywords.
# 🎨 泡泡玛特抖音评论分析：探索“扁平化”设计风格关键词 (Pop Mart Sentiment Analysis)

> **项目类型：** 数据分析、社交媒体挖掘 & 自然语言处理 (NLP)  
> **技术栈：** Python (Pandas, Matplotlib, WordCloud), Jieba (中文分词), Jupyter Notebook, 数据清洗

---

## 📖 1. 项目概述
在潮玩行业，理解消费者对产品设计的感性认知是品牌设计的核心。本项目以**泡泡玛特 (Pop Mart)** 在抖音平台上的用户评论为研究对象。

通过对大量用户评论进行数据抓取、清洗及情感倾向过滤，本项目重点提取了用户在描述产品时的**形容词**。目标是量化用户对“扁平化”设计风格（Flat Design）的感知，并识别出与之关联度最高的视觉与情感关键词，为产品迭代和市场营销提供数据驱动的洞察。

---

## 🗂️ 2. 仓库结构
本仓库的文件组织如下，确保分析流程的可追溯性：

    ├── data/
    │   └── douyin_popmart_comments.xlsx # 原始评论数据
    ├── notebooks/
    │   └── popmart_douyin_comment_analysis.ipynb                      # 核心分析脚本
    ├── images/
    │   ├── Top 10 Most Frequent Adjectives in Comments - Douyin.png   # 词频统计图
    │   └── Word Cloud of Adjectives in Comments - Douyin.png          # 词云图
    └── README.md                                                      # 项目说明文档

---

## 🛠️ 3. 核心流程
1.  **数据清洗 (Data Cleaning)**：去除重复评论及无效空值，过滤噪声文本。
2.  **分词与词性标注 (NLP Processing)**：利用 `jieba` 库进行中文分词，专门提取**形容词 (Adjectives)**，以捕捉用户对设计风格的定性评价。
3.  **情感聚焦 (Sentiment Focus)**：筛选正面评价，确保分析的关键词能够代表用户喜爱的设计特质。
4.  **可视化 (Visualization)**：生成词云图和高频词统计图表，直观呈现设计风格关键词。

---

## 📊 4. 可视化展示

### 关键形容词词频统计
通过对评论数据的挖掘，我们识别出了用户对产品感知最强的 10 个核心形容词。

![Top 10 Most Frequent Adjectives in Comments - Douyin.png](images/Top%2010%20Most%20Frequent%20Adjectives%20in%20Comments%20-%20Douyin.png)

### 关键词词云图
词云图展示了用户评价的分布，字号越大代表该设计特质在用户讨论中出现的频率越高。

![Word Cloud of Adjectives in Comments - Douyin.png](images/Word%20Cloud%20of%20Adjectives%20in%20Comments%20-%20Douyin.png)


---

## 💡 5. 关键洞察
基于对抖音评论的深度分析，我们识别出了用户对泡泡玛特产品感知最强的核心词汇：

* **温柔 (188次提及)** & **纯真 (153次提及)**：反映了色彩与线条带来的治愈感。
* **自由 (174次提及)** & **倔强 (164次提及)**：对应了 Zsiga 等系列独特的性格张力。
* **设计解读**：用户的评价呈现出明显的“情感化”倾向。除了视觉上的“好看”，用户更倾向于用带有性格特征的词汇来定义他们眼中的扁平化设计。

---

## ⚖️ 6. 伦理与局限
* **平台偏差**：抖音用户画像偏年轻化，分析结果主要代表该特定群体的审美趋势。
* **语义识别**：NLP 模型在处理复杂的中文网络梗时仍存在局限性，需结合人工抽样核验。

---

## 🚀 7. 未来工作
* **跨平台对比**：引入小红书 (Xiaohongshu) 数据，对比不同社区对设计风格认知的差异。
* **语义网络分析**：研究“温柔”等词汇常与哪些视觉元素共同出现，构建更精细的设计知识图谱。
