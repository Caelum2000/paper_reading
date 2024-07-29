## Title: LOFTQ: LORA-FINE-TUNING-AWARE QUANTIZA- TION FOR LARGE LANGUAGE MODELS
1. 通过初始化增强量化后需要用LoRA微调的模型的性能，特别是量化后bit比较少(<= 4)时候的性能
2. 初始化的objective是减少量化后权重加LoRA增加的权重之和与未量化的权重的误差，见Eq.6
3. 优化这个objective 是用迭代的方法，没有grad，见Algorithm.1
4. 使用SVD得到A,B的初始化估计值，从而减少Eq.6的objective. (为什么SVD有效？)