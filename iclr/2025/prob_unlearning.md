### A PROBABILISTIC PERSPECTIVE ON UNLEARNING AND ALIGNMENT FOR LARGE LANGUAGE MODELS
1. machine unlearning 是指使如LLM遗忘掉某些问题
2. 分析LLM输出的概率来检测是否unlearning成功的问题。本文argue之前的工作往往是分析确定的输出，这回导致分析不完全吗，可以使用某些attack方法得到unlearning 之前的信息（例如虽然需要遗忘的信息不是hardmax，但仍然有较大的概率）
3. 本文提出用entropy来regularize unlearning的loss，这样会使需要遗忘掉的信息不仅不会被hardmax选择，还会使其概率变小，在概率分布层面也不容易检测