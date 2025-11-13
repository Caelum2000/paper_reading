### On Causal and Anticausal Learning
1. 分析了不同情境下ML的因果层面的建模
2. anticausal是指，从effect学cause
3. 得出了一个主要结论，就是在半监督（SSL）且causal learning的情况下，给出额外的input信息（也就是cause信息）对学习没有作用。因为mechanism和cause是独立的。
4. 注意3中的结论，一个可以想到的反例是：假如我进行手写数字分类，那提供更多的手写数字样本我可以进行constrative representation learning，然后提升下游任务分类的性能。但这种情况手写数字样本是effect不是cause，因此是anticausal learning。这也表明anticausal learning对于SSL是有用的。