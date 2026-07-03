# 检索策略模板

## 目标
设计可复核的文献检索方案，为后续候选文献池和筛选记录提供来源依据。

## 建议输出

- 检索目标
- 目标数据库
- 关键词簇
- 组合检索式
- 时间范围
- 语言限制
- 候选池目标规模
- 导出文件说明

## 关键词组织建议

至少拆成三组：
1. 模型/方法词：LLM, foundation model, generative language model, GPT, Claude, Llama, domain LLM 等
2. 任务词：NER, RE, event extraction, summarization, QA, RAG, knowledge graph, hypothesis generation 等
3. 场景词：biomedical, clinical, medical, PubMed, EHR, literature, guideline, database 等

## 产物建议

- `检索策略.md`
- `检索式记录.md`
- `候选文献表.csv`
- `核心文献表.csv`
- 可选：采集结果 JSON

## 使用原则

- 不把“检索”与“筛选”混为一体
- 每次扩池都要留下增量记录
- 若后续发现证据缺口，应回到检索阶段补池，而不是直接在正文中硬写结论
