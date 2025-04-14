## From Coarse to Fine: Enable Comprehensive Graph Self-supervised Learning with Multi-granular Semantic Ensemble
1. 研究的是图自监督学习的问题
2. 采用了不同粒度的GNN，然后用ensemble 方法弄到一起
3. 使用了知识蒸馏的方法，这个需要调研
4. realted work应该会有用
5. 放waiting list


### review
1. GNN自监督+蒸馏。
2. teacher学到不同的prototype, 就是将不同的特征分散
3. 要求不同student（每个student对应一个prototype）和teacher的prototype的分散程度相同，见Eq.3 Eq.4
4. 将每个student做模型集成