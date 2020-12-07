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
* Machine Learning: k-NN / Naive Bayes / Decision Tree / k-means
* **DNN: word2vec / FastText / CNN / RNN / BERT**

### **Software Engineering**

* Service Develop: Python / PHP / Shell
* Middleware Apply: MySQL / Redis / Messge Queue / Hadoop
* Machine Learning Apply: TensorFlow / Keras / PyTorch

## Project Experience

### **Baidu Feed Short Text Antispam** `2018.5 - Present`

* Target: Detect malicious Ad, pornographic, insulting language from Baidu Feed comment, nickname, user sign, UGC text, etc.
* Ad Antispam<!-- : Data Normalize, Deform word recall, Deform text Reverse, Fasttext model training, Ad detect rule. -->
    1. Pretrain **word2vec** with comment corpus, trainning **fasttext** with **wordseg, pinyin** feature.
    `PR: 92% / 38% (+33% / +18%)`
    2. **Deform Text Reverse** for malicious Ad with similar character.
    `PR: 83% / 72% (-9% / +34%)`
    3. **Split long text** for malicious Ad with long harmless text.
    `PR: 85% / 80% (+2% / +8%)`
    4. **Remove radical** for malicious Ad with deformed character by adding radical.
    `PR: 83% / 78% (-2% / -2%), Malicious Ad solve 60%`
    5. Embedding with **Chinese charcter component**.
    `PR: 85% / 84% (+2% / +6%), Malicious Ad solve 100%`
* Porn & Insult Antispam
    1.  Training Fasttext, CNN, BERT ensemble classifier.
    `PR: 60% / 61% (+3% / +4%)`
    2.  Use **title-comment** sentence pair for BERT NSP pretrain. Finetuning BERT with more labeled corpus.
    `PR: 79% / 64% (+19% / +3%)`
* Result: Keep spam rate on random page < 0.5%, and spam rate on top 50 page daily < 0.5%

### **Baidu Feed Low Quality Langurage Detection** `2019.9 – Present`

* Target: Detect low quality langurage (defaming original poster, defaming famous, copy comment, messy code, etc.) from Baidu Feed comment, UGC text.
* Personal Work: Comment target identification. Adding emotion feature. Adding messy code detect rule.
* Result: Reduce low quality rate on random page from 13.3% to 9% (-3.3%), low quality rate on top 50 page from 10.4% to 10.1% (-0.3%)

### **Baidu Feed Antispam Service Development** `2017.7 – 2018.2`

* Target: Develop Baidu Feed antispam service, support BaiJiaHao(百家号) PGC, UGC content antispam.
* Personal Work: Service framework design (PHP, BigPipe, DStream) & development. Adding keyword realtime configuration ability.
* Result: Support Baidu Feed antispam with 200k+ query daily.

<!-- ### **相关知识推荐，策略研发** `2017.5 – 2017.6 `

* Target: 百度feed文章落地页添加相关知识推荐卡片槽位，展示文章主题相关的百科词条。
* Personal Work: 数据流接入，主题模型效果调优。
* Result: 百科知识模块分发2.6万，展现226万（占feed全量0.5%），点展比1.33%；召回百科落地页平均时长+0.9秒/每篇(+1.23%)；
 -->
### **Baidu Hotel Guarantee Prepay API Development** `2017.3 – 2017.4`

* Target: Support hotel room rate & guarantee prepay and refund online. Sync capital pool with Baidu Payment. Sync hotel info with TPs.
* Personal Work: Project schedule management. Service framework design (client, business, payment, order module). Payment module development.
* Result: Support 18500+ hotel guarantee prepayment.
	- Hotel occupancy increase 3%, order room-night increase 1.85%.
	- Guarantee prepay order quantity > 350, GMV > 94000 RMB daily. Guarantee prepay 15.25%, is 3.55% more than Ctrip(携程旅行).

<!-- ### **酒店商家自促，服务端研发接口人** `2016.12 – 2017.1`

* Target: 支持酒店商家线上预定流程自营销，同时获取C端优质曝光位。
* Personal Work: 项目管理；系统架构设计，营销模块商家资金池开发。

### **酒店营销平台，服务端研发负责人** `2015.7 – 2016.11`

* Target: 支持代金券优惠、下单立减等运营功能。
* Personal Work: 技术优化5+项（API并行化、异步等）；平台功能扩展10+项（随机、周期、推送、下单分享等）
* Result: API平响从秒级优化至毫秒级，运营活动迭代从周级缩短至2天，扩展至3个业务线，运营关联订单GMV14.72亿（2016上半年）

### **机票预订，服务端研发** `2015.12`

* Target: 接入携程机票预订业务。
* Personal Work: 系统架构设计，订单中心模块功能实现。

### **分布式流程控制引擎，服务端研发** `2014.10 – 2014.12`

* Target: 基于DAG的任务自动化处理服务。
* Personal Work: 任务调度DAG流程设计，任务调度引擎开发。
* Result: 地图内业工艺整体流程时间从天级减少至8h内。

### **百度地图内业数据管理系统，服务端研发** `2014.4 – 2014.12`

* Target: 支持底图数据内业生产流程。
* Personal Work: 流程优化，接入数据工具10+项，系统功能实现。
 -->