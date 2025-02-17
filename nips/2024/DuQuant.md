## DuQuant: Distributing Outliers via Dual Transformation Makes Stronger Quantized LLMs
1. 通过选出outlier activation来进行更好的quant
2. 放进waiting list


### review
1. 将outlier分为两类，一种是normal outlier 是一个channel都过大，另一种是massive outlier只有单个数值过大，见Figure.1
2. 使用旋转和置换变化来将这两种outlier变得均匀，见Figure.2