## Provable Multi-Task Representation Learning by Two-Layer ReLU Neural Networks
1. 主要是研究pretraining的model上能否学到普遍的表征
2. 使用了一个toy model，两层中间有一个ReLU的MLP，通过multi-task 看第一层是否能学到表征
3. 结论：第一层能学到表征；在固定浅层，并在不同task下微调输出头的multi task loss可以是一个constrative loss