## Introducing Language Guidance in Prompt-based Continual Learning
1. 用语言encoder指导prompt pool的分布，使用的方法是类似对比学习的loss
2. 问题：prompt pool的选择网络，就是将input映射到key空间的网络是怎么对齐语言encoder的表征的？