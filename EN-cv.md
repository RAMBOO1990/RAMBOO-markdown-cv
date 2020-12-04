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

* Master degree, Software Engineering
* Major in Mobile Internet & Game Engineering

### **GuiZhou University** `2009.9 - 2013.6`

```
GuiZhou, China
```

* Bachelor's degree, Computer Science

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

### **Baidu** `2015.7 - Present`

```
BeiJing, China
```

* NLP Engineer
* Software Engineer

### **Baidu Intern** `2014.4 - 2014.12`

```
BeiJing, China
```

* Software Engineer

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

### **Baidu Feed NLP Antispam** `2018.5 - Present`

* Target: Detect malicious Ad, pornographic, insulting language from Baidu Feed comment, nickname, user sign, UGC text, etc.
* Ad Antispam: Data Normalize, Deform word recall, Deform text Reverse, Fasttext model training, Ad detect rule.
    1. **word2vec** pretrain with Feed comment corpus, train **fasttext** for classifier. Add **wordseg, pinyin** feature.
    `PR: 92% / 38% (+33% / +18%)`
    2. **Deform Text Reverse** for malicious Ad with similar character.
    `PR: 83% / 72% (-9% / +34%)`
    3. **Split long text** for malicious Ad with long harmless text.
    `PR: 85% / 80% (+2% / +8%)`
    4. **Remove radical** for malicious Ad with deformed character by adding radical.
    `PR: 83% / 78% (-2% / -2%), Malicious Ad solve 60%`
    5. Embedding with **Chinese charcter component**.
    `PR: 85% / 84% (+2% / +6%), Malicious Ad solve 100%`
* Porn & Insult Antispam:
    1.  Training Fasttext, CNN, BERT ensemble classifier.
    `PR: 60% / 61% (+3% / +4%)`
    2.  Use **title-comment** sentence pair for BERT NSP pretrain. Add labeled corpus for BERT Finetune.
    `PR: 79% / 64% (+19% / +3%)`
* Result: Keep spam rate on random page < 0.5%, and spam rate on top 50 page daily < 0.5%

### **Baidu Feed NLP Low Quality Text Detection** `2019.9 – Present`

* Target: Detect low quality langurage (defaming original poster, defaming famous, copy comment, messy code, etc.) from Baidu Feed comment, UGC text.
* Personal Work: Identification comment target, add emotion feature, add messy code detect rule.
* Result: Reduce low quality rate on random page from 13.3% to 9% (-3.3%), low quality rate on top 50 page from 10.4% to 10.1% (-0.3%)
