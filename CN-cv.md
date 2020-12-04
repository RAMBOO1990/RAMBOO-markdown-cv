---
layout: cv
title: RAMBOO CV
phone: 170-9041-7441
email:
  url: mailto:ramboooo@126.com
  text: ramboooo@126.com
---

# 袁晖

<!--
include contact information from the front matter
Supported arguments:
    - homepage: url, text
    - phone
    - email
-->

{% include cv-contact.html %}

## 教育经历

### **浙江大学** `2013.9 - 2015.6`

```
浙江，中国
```

- 软件工程，硕士学位
- 研究方向：移动互联网与游戏开发

### **贵州大学** `2009.9 - 2013.6`

```
贵州，中国
```

- 计算机科学，学士学位

## 曾获荣誉

百度LBS 2016最佳团队 <br>
贵州大学程序设计大赛一等奖 <br>
贵州大学程序设计大赛一等奖 <br>
全国青少年信息学奥林匹克联赛（广东赛区）二等奖 <br>
全国青少年信息学奥林匹克联赛（广东赛区）三等奖 <br>
全国青少年信息学奥林匹克联赛（广东赛区）二等奖 <br>
全国青少年信息学奥林匹克联赛（广东赛区）三等奖 <br>
全国青少年信息学奥林匹克联赛（广东赛区）三等奖 <br>

## 工作经验

### **百度** `2015.7 - 至今`

* NLP策略工程师 `2017.6 - 至今`
* 研发工程师 `2015.7 - 2017.6`

### **百度(实习)** `2014.4 - 2014.12`

* 研发工程师

## 专业技能

### **算法**

* **基础（精通）: 贪心 / 递归 / 排序 / 二分**
* **数据结构（熟悉）: 树状数组 / 哈希表 / 堆**
* **树遍历（精通）: 广搜 / 深搜**
* **图论（熟悉）: 联通性 / 最短路 / 拓扑排序**
* 数论（了解）: 博弈论 / 组合数学
* 动态规划（了解）: 背包问题 / 记忆化搜索
* **深度神经网络（熟悉）: word2vec / FastText / 卷积神经网络 / 循环神经网络 / BERT**
* 机器学习（了解）: k近邻 / 朴素贝叶斯 / 决策树 / k均值

### **软件工程**

* 服务端研发: Python / PHP / Shell
* 中间件应用: MySQL / Redis / Messge Queue / Hadoop
* 机器学习应用: TensorFlow / Keras / PyTorch

## 项目经历

### **Feed短文本反作弊策略研发 Baidu Feed NLP Antispam** `2018.5 - 至今`

* 项目背景：识别并过滤短文本的广告、色情、辱骂文本内容，主要业务场景为百度Feed信息流评论，并已输出至百度视频弹幕、用户签名、用户昵称、百度贴吧等业务。
* 广告反作弊策略优化：数据归一化、变体词召回、变体还原、模型识别、规则识别。模型迭代自动化，联合搜索业务封禁黑产域名。
    1. 使用大量feed评论语料预训练词向量，使用**fasttext**训练分类模型；添加**单字、分词、拼音**特征；增加训练数据。
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