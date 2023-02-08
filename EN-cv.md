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

* Back-end Develop: Python / PHP / Shell
* Middleware Apply: MySQL / Redis / Messge Queue / Hadoop
* Machine Learning Apply: TensorFlow / Keras / PyTorch

## Project Experience

### **Overseas SPU Same Style & Price Comparison** `2022.03 - 2022.08`

* Project Background: Expansion of overseas e-commerce business requires support from commodity same-style ability to address shortage and price comparison in merchant business. Due to cross-language and poor infrastructure for overseas e-commerce, such as basic attributes.
* Individual Work:
    - Constructing key attributes for comparison, such as model, set, quantity, size, weight, and capacity, and promoting the optimization of SPU attributes such as category and brand at a granular level
    - Establishing key attribute configuration to support attribute matching at different granularities
    - Incorporating SPU same-style models to assist in multilingual text same-style matching effects
* Results: Based on the Arctic goods inventory in Indonesia in July/August, the accuracy of the shortage SPU increased from 60% to 69%, the accuracy of SPU same-style recall increased from 73%/57% to 79%/60%, and the accuracy of comparable prices increased from 65% to 82%.
    - Accuracy of key attribute matching for comparison increased from 84.13%/68.67% to 83.08%/96.95%.
    - End-to-end accuracy recall increased from 77.80%/69.79% to 77.96%/96.95%.
    - TTS price advantage rate increased from 56.86% to 60.08%.
    - TTS non-disadvantage price rate increased from 62.86% to 65.69%.

### **Digital SPU Same-item Strategy Optimization** `2021.06 - 2022.02`

```
Project Owner
```

* Project Background: In the 3C digital household appliances industry, the same digital items are recognized at the SPU granularity.
* Individual work: Overall strategies are formulated from two aspects of the product: product level and information quality.
    - Product level: accessory recognition (category, keywords), abnormal price differences, brand level, category, etc.
    - Product information quality: sets, disorder, attribute conflicts (self-filled attributes, title, different models in pictures), etc.
    - For standardized and high-quality information products, more text-structured features are used (stricter brand, category, and model judgments); for non-standardized and low-quality information products, more picture features are used (higher whole picture, first picture, and similarity threshold of picture subjects).
    - Basic attribute optimization (SKU title recognition model, etc.), feature matching strategy optimization (title supplement model suffix, model suffix compatibility, editing distance compatibility, etc.).
* Results: 3C digital household appliances market recall 92.31%/54.78%; recall in the same store 87.22%; validation set recall 94.36%/73.22%.


### **SPU Same-Style Strategy** `2021.03 - present`
* Project Background: Identify SPU same-style products, construct SPU same-style clusters, and provide SPU same-style capabilities for product same-style recommendation, search, deduplication, richness shortage judgment, and other business services.
* Personal Work:
    - Optimize SPU cluster features to increase coverage to 99%+, and enhance product cluster recall ability.
        + Accuracy of first-level category in cluster category 93% (+3%), accuracy of second and third-level categories 77%
        + Accuracy of cluster keywords increased from 38% to 77% (+39%), recall improved from 56% to 63% (+7%), and built own product keywords.
        + Accuracy of cluster brand 93%.
    - Optimized product cluster recall: Product-Cluster Keyword Single Recall 94.81%, Product-Product Recall 88% to 91% (+3%).
    - Refactored product cluster similarity service to reduce calculation and improve service performance.
    - Built same-style sort service with optimized features.
* Results: Sorted out different industry cluster features, recall accuracy improved significantly to 90%+, and SPU product cluster similarity service performance improved significantly, QPS increased from 100 to 500+.


### **Construction of the sku deduplication cluster pipeline** `2021.10 - 2022.02`

* Project Background: Based on the current SPU cluster capability, the SKU-level same-type capability is provided for the product comparison business through the fine-grained SKU clustering.
* Personal Work: Designing the overall solution for sku deduplication, building cluster mounting, sku cluster bucket, cluster similarity, and cluster feature update services, and integrating the entire pipeline process.
* Results: The sku deduplication cluster was built with an MVP solution, with an overall pipeline QPS of 500+ and a pct999 delay of 5s-.


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
    `PR: 83% / 78% (-2% / -2%). Malicious Ad solve 60%`
    5. Embedding with **Chinese charcter component**.
    `PR: 85% / 84% (+2% / +6%). Malicious Ad solve 100%`
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
* Personal Work: Back-end architecture design (PHP, BigPipe, DStream) & development. Adding keyword realtime configuration ability.
* Result: Support Baidu Feed antispam with 200k+ query daily.

<!-- ### **相关知识推荐，策略研发** `2017.5 – 2017.6 `

* Target: 百度feed文章落地页添加相关知识推荐卡片槽位，展示文章主题相关的百科词条。
* Personal Work: 数据流接入，主题模型效果调优。
* Result: 百科知识模块分发2.6万，展现226万（占feed全量0.5%），点展比1.33%；召回百科落地页平均时长+0.9秒/每篇(+1.23%)；
 -->
### **Baidu Hotel Guarantee Prepay Service Development** `2017.3 – 2017.4`

* Target: Support hotel room rate & guarantee prepay and refund online. Sync capital pool with Baidu Payment. Sync hotel info with TPs.
* Personal Work: Project schedule management. Back-end architecture design (client, business, payment, order module). Payment module development.
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