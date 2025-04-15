## LCA-on-the-Line: Benchmarking Out-of-Distribution Generalization with Class Taxonomies
1. 预测模型的Out-of-Distribution (OOD) performance
2. ICML有OOD的tutorial
3. 放waiting list


### review
1. 很insightful，没太多数学
2. 提出了一种方法LCA，来度量模型的OOD能力，这样就不需要在OOD数据集上进行测试
3. 指出了VM(vision model)和VLM在泛化OOD能力上的差异，同样的ID(in-distribution) acc下，VLM的OOD更好
4. LCA看被模型误分类的data是否和ground truth在语义树上相似，这里使用的语义树是wordnet。具体度量两个节点的距离方法是看共同祖先节点与ground truth的距离，见Fig.3
5. 问题1：为什么LCA能度量OOD的能力？答：因为语义树去除了图像模态的如背景等无关因素对模型的影响，仅保留语言。而背景，颜色风格是影响VM的OOD的关键
6. 问题2：为什么VLM比VM OOD能力强。答：VLM对齐了语言的表示，所以能去除一些图像模态不需要的特征的影响（如背景，风格），从而提取抽象的语言结构