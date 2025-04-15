## Test-Time Model Adaptation with Only Forward Passes
1. 提出一种基于边缘端，高效的adaptation方法
2. 具体不知道干什么的
3. 放waiting list


### review
1. 研究的是test time adaption问题，就是模型在训练的时候是一个data distribution, 但是在实际应用的时候（test time）就可能OOD，这时候需要后训练一次model，使其adapt 这个偏移的test distribution
2. 本文主要是针对边缘场景，没有足够的算力进行TTA训练
3. 对ViT输入新的prompt，并且只学习这个prompt，减小计算量
4. 没有使用BP，使用了一种CAS演化的方法，减少开销