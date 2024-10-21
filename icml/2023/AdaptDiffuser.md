## Title: AdaptDiffuser: Diffusion Models as Adaptive Self-evolving Planners
1. 利用diffusion生成state-action序列
2. 利用了reward做guidance
3. 有一个discrimiantor, 来分辨序列的好坏
4. 生成的序列根据状态转移矩阵进行筛选（具体怎么筛选的写的不太详细）