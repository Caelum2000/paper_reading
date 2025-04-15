## Discovering Environments with XRM
1. 解决 out-of-distribution (OOD) generalization 问题
2. 好像是关于环境标注的，不太懂
3. ICML有OOD的tutorial
4. 放到waiting list


### review
1. 一些OOD的算法需要对环境进行标注，因为要想泛化需要去除环境对“真正的”feature的影响
2. 本文主要是关注环境“自动标注”，消除人力的影响
3. 使用两个网络，然后根据分类准确率的差异来决定是哪个环境（因为环境会影响分类准确率）