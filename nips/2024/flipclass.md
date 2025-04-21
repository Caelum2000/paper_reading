## Flipped Classroom: Aligning Teacher Attention with Student in Generalized Category Discovery
1. 研究内容是利用self-supervise learning 解决 Generalized Category Discovery (GCD)问题
2. GCD是根据已经学习到的标签来识别未知标签的组合物体，这个需要调研一下
3. 放waiting list, 主要是调研GCD相关内容


### review
1. 解决GCD问题，就是一个相对general的teacher 教给 student在更general的open world中进行任务，具体看Eq.1的解读
2. 发现这种范式效果不好，指出是teacher和student的特征没align
3. 用hopfield network的能量函数来对齐特征，但感觉这个故事性大于实际意义