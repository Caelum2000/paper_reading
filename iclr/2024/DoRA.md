## IS IMAGENET WORTH 1 VIDEO? LEARNING STRONG IMAGE ENCODERS FROM 1 LONG UNLABELLED VIDEO
1. 借鉴了DINO的思想，设计了一种通过video自监督的学习方法
2. 提供了一个video的数据集
3. 有一个产生object mask的方法，较为复杂。主要目的是使teacher和student有不同的scale（通过mask获得更local的特征）
4. 在downstream任务上可以与imagenet pretrain的model相比