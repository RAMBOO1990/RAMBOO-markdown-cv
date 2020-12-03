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

## Education

### **ZheJiang University** `2013.9 - 2015.6`

```
ZheJiang, China
```

- Master Degree, Software Engineering
- 研究方向：移动互联网与游戏开发

### ** GuiZhou University** `2009.9 - 2013.6`

```
GuiYang, China
```

- B.S., Computer Science

## Honors & Awards

Baidu LBS 2016 Best Team Award `Baidu, 2017.1` <br>
GZU ICPC First Prize `GuiZhou University, 2012.6` <br>
GZU ICPC First Prize `GuiZhou University, 2011.6` <br>
NOIP (GuangDong) Second Prize `GuangDong, 2009.11` <br>
NOIP (GuangDong) Third Prize `GuangDong, 2008.11` <br>
NOIP (GuangDong) Second Prize `GuangDong, 2007.11` <br>
NOIP (GuangDong) Third Prize `GuangDong, 2006.11` <br>
NOIP (GuangDong) Third Prize `GuangDong, 2005.11` <br>

## Work Experience

### **Baidu R&D** `2015.7 -`

### **Baidu R&D Intern** `2014.4 - 2014.12`

## Professional Skills

### **Algorithm**

* **Base: Greedy / Recursive / Sort / Bisection Search**
* **Data Structure: Binary Indexed Tree / Hash Table / Heap**
* **Tree Search: DFS / BFS**
* **Graph Theory: Connectedness / Shortest Path / Topological Sorting**
* Number Theory: Game Theory / Combinatorial Mathematics
* DP: Knapsack Problem / Memorize Search
* **DNN: word2vec / FastText / CNN / RNN / BERT**
* Machine Learning: k-NN / Naive Bayes / Decision Tree / k-means

### **Software Engineering**

* Service Develop: Python / PHP / Shell
* Middleware Apply: MySQL / Redis / Messge Queue / Hadoop
* Machine Learning Apply: TensorFlow / Keras / PyTorch

## Project Experience

### **Baidu Feed NLP Antispam** `2018.5 - `

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

