# 代表与前沿研究

核验截止2026-10-02。10项入口兼顾经典方法和2025–2026选定研究，不是医学AI全景或效果榜。基础模型、影像恢复、单细胞解释、医学视觉问答是不同任务；论文中的“优于已有方法”仅在其测试设置内成立。

|研究|时间与状态|阅读价值|来源与边界|
|---|---|---|---|
|U-Net，Ronneberger等|2015-05-18预印本；经典医学分割方法|理解编码器、解码器、跳跃连接和少标注情形|[作者原文](https://arxiv.org/abs/1505.04597)，原任务成绩不证明所有医疗分割通用|
|Geneformer：Transfer learning enables predictions in network biology|Nature2023，正式论文|单细胞预训练如何支持有限数据下的网络生物学任务|[正式文章](https://www.nature.com/articles/s41586-023-06139-9)，关注预训练来源及下游任务隔离|
|scGPT|Nature Methods2024，正式论文；21:1470–1480|生成式预训练与多种单细胞下游任务；scKAN教师背景|[正式文章](https://www.nature.com/articles/s41592-024-02201-0)，不同zero-shot/fine-tune协议不能混比|
|Mamba：Linear-Time Sequence Modeling with Selective State Spaces|2023-12-01首投预印本|理解状态空间与选择机制，作为HiCMamba方法背景|[原文](https://arxiv.org/abs/2312.00752)，通用序列结果不直接证明Hi-C效果|
|Mixed Prototype Correction for Causal Inference in Medical Image Classification，P364|ACM MM2024正式论文，PDF有会议信息|原型、中介与前门调整；检查因果条件|[DOI](https://doi.org/10.1145/3664647.3681395)，本篇读摘要，非因果识别条件全面审计|
|Consensus representation of multiple cell–cell graphs…，P361/scMCGraph|2025-01-23，正式期刊论文|多通路视图、共识图与跨数据注释|[正式文章](https://doi.org/10.1186/s12915-025-02128-8)，阅读证据为摘要与框架，不将全篇称精读|
|scKAN，P354|Genome Biology2025，26:300|scGPT蒸馏、KAN曲线与标志基因；读第1–5页|[正式DOI](https://doi.org/10.1186/s13059-025-03779-0)，药物案例的分子动力学不是临床验证|
|HiCMamba，P344|PLOS Computational Biology2026-03-24正式；预印本2025-03-13|多尺度状态空间、Hi-C接触图增强及结构评价|[正式文章](https://journals.plos.org/ploscompbiol/article?id=10.1371/journal.pcbi.1014057)，已读PDF第1、3–5页；不同细胞系与降采样需分别验证|
|Better Eyes, Better Thoughts，P365|arXiv2026-03-02首投；v2为2026-04-10，预印本|医学VQA直接回答与CoT比较、RoI和描述干预|[arXiv](https://arxiv.org/abs/2603.06665)，感知瓶颈是研究假设，不能推广到全部医学推理|
|AbLWR，P366|arXiv2026-04-13；预印本，未核验正式接收|抗体亲和力列表排序、PU学习与同源抗原采样|[arXiv论文](https://arxiv.org/abs/2604.11272)，已读摘要；随机交叉验证不替代新抗原外推|

## 近期补充线索

[Geneformer规模与量化研究](https://www.nature.com/articles/s43588-026-00972-4)为Nature Computational Science2026正式研究，提出资源效率与生物预测结合的方向；本篇只核验公开摘要/页面，未读取其完整实验，不写具体速度或泛化结论。它可以帮助判断“更大预训练”与“轻量可解释学生”各自解决什么问题。

scBIT为第三篇核心方法材料，见[作者稿](https://arxiv.org/abs/2502.02630)。索引标2026-03-19，作者稿不一定保留正式卷期；本篇已读第1–5页理解跨个体辅助配对，正式引用前需根据索引DOI复核出版页和版本。

## 查文献时的易错点

“scKAN”搜到的胰腺分割SCKAN、另一组基因网络推断scKAN，均不可冒认作黄志安的单细胞解释论文。应同时核对标题、作者、DOI。scGraphPilot与Functionally Guided Graph Learning可能有版本关系，但在未核对全文和DOI前保留独立记录。



## 研究假设需要怎样验证

选择一个独立性单位：患者、医院、细胞系或抗原；明确一个失效模式：批次效应、稀有类型、未见突变或结构幻觉；采用两类指标：预测质量和领域保真。解释性结果再加入重复运行稳定性及独立领域证据。所有候选基因、药物与机制推断先以候选称呼，按计算、体外、动物和临床层级分别报告。

## 扩展代表文献与版本

本表列出直接论文来源与版本状态，预印本与正式发表分别记录。

| 论文 | 已核验来源 | 发表与版本状态 | 阅读依据 |
|---|---|---|---|
| [Confidence Calibration under Ambiguous Ground Truth](../papers/P060.md) | [直接来源](<https://arxiv.org/abs/2603.22879v1>) | 已核 arXiv 预印本；官方摘要页未见会议/期刊发表声明，本次未确认正式发表。 | fulltext |
