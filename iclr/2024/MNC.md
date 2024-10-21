## MULTI-GRANULARITY CORRESPONDENCE LEARNING FROM LONG-TERM NOISY VIDEOS
1. 利用最优传输实现video-caption时间对齐
2. 先计算video和caption的相似性矩阵，然后离散最优传输
3. 采用了对比学习的方法，见Eq.4
4. 不用粒度的学习，有视频之间的也有一个视频内不同batch的对比学习