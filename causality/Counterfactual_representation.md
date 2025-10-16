### Title: Learning Representations for Counterfactual Inference
1. 本论文的目标是在给定样本以及treatment的情况下，学到一个encoder。
2. 这个encoder能够提取样本中与treatment无关的特征，并通过该特征以及treatment预测output
3. 公式(2)是主loss，分为3部分。第一部分是预测的loss，第二部分是为了让特征分布和treatment无关(balance). 第三部分是为了使特征能对反事实进行预测。
4. 注意Section 4.1表明，balance部分可以简化成treatment=1/0的特征差异