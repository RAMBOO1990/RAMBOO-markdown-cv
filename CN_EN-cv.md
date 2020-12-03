---
layout: cv
title: RAMBOO CV
phone: 170-9041-7441
email:
  url: mailto:ramboooo@126.com
  text: ramboooo@126.com
---

# 袁晖 YuanHui

<!--
include contact information from the front matter
Supported arguments:
    - homepage: url, text
    - phone
    - email
-->

{% include cv-contact.html %}

## 教育经历 Education

### **浙江大学 ZheJiang University** `2013.9 - 2015.6`

```
浙江 ZheJiang, China
```

- 软件工程，硕士学位 Master Degree, Software Engineering
- 研究方向：移动互联网与游戏开发

### **贵州大学 GuiZhou University** `2009.9 - 2013.6`

```
贵阳 GuiYang, China
```

- 计算机科学，学士学位 B.S., Computer Science

## 曾获荣誉 Honors & Awards

百度LBS 2016最佳团队 Baidu LBS 2016 Best Team Award `Baidu, 2017.1` <br>
贵州大学程序设计大赛一等奖 GZU ICPC First Prize `GuiZhou University, 2012.6` <br>
贵州大学程序设计大赛一等奖 GZU ICPC First Prize `GuiZhou University, 2011.6` <br>
全国青少年信息学奥林匹克联赛（广东赛区）二等奖 NOIP (GuangDong) Second Prize `GuangDong, 2009.11` <br>
全国青少年信息学奥林匹克联赛（广东赛区）三等奖 NOIP (GuangDong) Third Prize `GuangDong, 2008.11` <br>
全国青少年信息学奥林匹克联赛（广东赛区）二等奖 NOIP (GuangDong) Second Prize `GuangDong, 2007.11` <br>
全国青少年信息学奥林匹克联赛（广东赛区）三等奖 NOIP (GuangDong) Third Prize `GuangDong, 2006.11` <br>
全国青少年信息学奥林匹克联赛（广东赛区）三等奖 NOIP (GuangDong) Third Prize `GuangDong, 2005.11` <br>

## 工作经验 Work Experience

### **百度研发工程师 Baidu R&D** `2015.7 -`

### **百度研发工程师(实习) Baidu R&D Intern** `2014.4 - 2014.12`

## 专业技能 Professional Skills

### **算法 Algorithm**

* **基础（精通） Base: 贪心 Greedy / 递归 Recursive / 排序 Sort / 二分 Bisection Search**
* **数据结构（熟悉） Data Structure: 树状数组 Binary Indexed Tree / 哈希表 Hash Table / 堆 Heap**
* **树遍历（精通） Tree Search: 广搜 DFS / 深搜 BFS**
* **图论（熟悉） Graph Theory: 联通性 Connectedness / 最短路 Shortest Path / 拓扑排序 Topological Sorting**
* 数论（了解） Number Theory: 博弈论 Game Theory / 组合数学 Combinatorial Mathematics
* 动态规划（了解） DP: 背包问题 Knapsack Problem / 记忆化搜索 Memorize Search
* **深度神经网络（熟悉） DNN: word2vec / FastText / 卷积神经网络 CNN / 循环神经网络 RNN / BERT**
* 机器学习（了解） Machine Learning: k近邻 k-NN / 朴素贝叶斯 Naive Bayes / 决策树 Decision Tree / k均值 k-means

### **软件工程 Software Engineering**

* 服务端研发 Service Develop: Python / PHP / Shell
* 中间件应用 Middleware Apply: MySQL / Redis / Messge Queue / Hadoop
* 机器学习应用 Machine Learning Apply: TensorFlow / Keras / PyTorch

## 项目经历 Project Experience

### **Feed短文本反作弊策略研发 Baidu Feed NLP Antispam** `2018.5 - `

* 项目背景：识别并过滤短文本的广告、色情、辱骂文本内容，主要业务场景为百度Feed信息流评论，并已输出至百度视频弹幕、用户签名、用户昵称、百度贴吧等业务。
* 广告反作弊策略优化：数据归一化、变体词召回、变体还原、模型识别、规则识别。模型迭代自动化，联合搜索业务封禁黑产域名。
    1. 使用大量feed评论语料预训练词向量，使用**fasttext**训练分类模型；数据预处理环节添加**单字、分词、拼音**特征；训练数据集增加众测数据。
    `准召：92% / 38% (+33% / +18%)`
    2. 数据预处理阶段加入**变体还原**策略，对黑产变体case进行数据清洗；形近字数据增强。
    `准召：83% / 72% (-9% / +34%)`
    3. 长文本分割策略，解决黑产冗余文本case。
    `准召：85% / 80% (+2% / +8%)。`
    4. 添加去部首变体，输入序列加入字形特征。
    `准召：83% / 78% (-2% / -2%)。黑产case解决率60%。`
    5. embedding加入字形特征，提升形近字泛化能力。
    `准召：85% / 84% (+2% / +6%)。黑产case解决率100%。`
* 色情、辱骂反作弊策略优化：
    1. fasttext + cnn + bert多模型融合。
    `准召：60% / 61% (+3% / +4%)`
    2. 使用“标题-评论”sentence-pair进行预训练任务，引入标题语境特征。例行添加标注样本，迭代模型。
    `准召：79% / 64% (+19% / +3%)`
* 成果：始终保持线上随机文章评论及热门文章top评论残留率在0.5%以内；提高了广告反作弊策略泛化能力，将模型迭代周期从月级缩短至周级，增加黑产作弊成本。

* Project Background: Check & Delete malicious Ad, porn, insult content in Baidu Feed comment, nickname, user sign, UGC text etc.
* Ad Antispam: Data Normalize, Deform word recall, Deform text Reverse, Fasttext model training, Ad check rule.
    1. **word2vec** by comment corpus, train **fasttext**. Add **wordseg, pinyin** feature.
    `precision 92% / recall 38% (+33% / +18%)`
    2. **Deform Text Reverse** for malicious Ad with similar character.
    `precision 83% / recall 72% (-9% / +34%)`
    3. **Split long text** for malicious Ad with long harmless text.
    `precision 85% / recall 80% (+2% / +8%)`
    4. **Remove radical** for malicious Ad with deformed character by adding radical.
    `precision 83% / recall 78% (-2% / -2%), solve malicious Ad bad case 60%`
    5. Embedding with **Chinese charcter component**.
    `precision 85% / recall 84% (+2% / +6%), solve malicious Ad bad case 100%`
* Porn & Insult Antispam:
    1.  training Fasttext, CNN, BERT ensemble.
    `precision 60% / recall 61% (+3% / +4%)`
    2.  Use "title-comment" sentence pair for BERT NSP pretrain, add title feature. Add more labeled corpus for BERT Finetune.
    `precision 79% / recall 64% (+19% / +3%)`
* Result: Keep spam rate on random page < 0.5%, and spam rate on top 50 page daily < 0.5%

