## APT: Adaptive Pruning and Tuning Pretrained Language Models for Efficient Training and Inference
1. 在用LoRA finetune的同时对模型参数进行剪枝
2. 背后的需求是：LoRA会增加参数量，所以剪枝来抵消这一部分参数量
3. 之前有类似的工作(Sec2.3 + AdaLoRA)。这个文章主要讲自己高效