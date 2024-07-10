## Title: SPATIO-TEMPORAL APPROXIMATION: A TRAINING- FREE SNN CONVERSION FOR TRANSFORMERS
1. ANN-SNN 转换，能够转换transformer
2. 对于transformer里的GLUE，先用ANN+RELU学习一个GLUE的近似，然后再用转换RELU的方法转换
3. 对于transformer的QK^T. 提出一套估计方法，据论文说比直接估计高效，但这一点存疑，还需要讨论    