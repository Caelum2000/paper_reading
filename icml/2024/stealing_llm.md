## Stealing Part of a Production Language Model
1. 获取LLM最后一层输出的投影矩阵的rank甚至是确切的矩阵值
2. 前提条件是LLM的API能够返回transformer输出的logits (这用于控制条件生成，因此一般API都有)
3. 获取最后一层投影矩阵W的rank的方法是对logits组成矩阵Q进行SVD，这样rank_Q=rank_W。这是因为一般词表的大小远大于rank_W
4. 获取W具体值的方法是进行最小二乘回归，具体见Sec 4.2
5. 文章讨论了只有部分logits的时候这么办(比如top-5)。具体方法是对词表加Bias，见Sec 5.1。前提条件是API允许这样做
6. 讨论了返回softmax后的logprobs而不是logits怎么做，见sec 5.2