## DN-DETR: Accelerate DETR Training by Introducing Query DeNoising
1. 指出之前版本的DETR收敛慢的原因在于生成anchor的对应关系会变化，因此导致收敛慢
2. 提出用加了noise 的ground truth训练，以解决上述问题
3. 采用attention mask进行隔离，从而在训练的过程中加入没有ground truth anchor的learnable anchor. 因为推理的时候是完全不知道ground truth的，因此不能得到加噪声的label
4. 具体实现得看代码，论文有点具体细节不清楚