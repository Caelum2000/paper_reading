### Title: Estimating individual treatment effect: generalization bounds and algorithms
1. 和Learning Representations for Counterfactual Inference类似，都是从不同treatment的数据中学到和treatment无关的feature。
2. 然后用这个feature进行反事实的预测
3. 本文和Learning Representations for Counterfactual Inference不同的是，loss里的balance部分使用积分距离IPM代替，如MMD。另外推出了一些bound

 