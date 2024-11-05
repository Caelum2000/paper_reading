## INFOBATCH: LOSSLESS TRAINING SPEED UP BY UNBIASED DYNAMIC DATA PRUNING
1. 通过对数据进行剪枝（筛选数据）来对训练进行加速
2. 本文是动态的剪枝方法，即每个epoch筛选掉一些无效的数据，每个epoch的threshold会变
3. 每个epoch后对数据集计算loss来确定score，然后根据score的平均值作为threshold来筛选