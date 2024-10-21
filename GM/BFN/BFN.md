## Title: Bayesian Flow Networks
1. 通过不断更新离散的pdf参数，来建模概率。这样的好处是即使data是离散的，也会有连续的参数
2. 有一个sender(真实的data)，和receiver(通过优化参数来生成fake data). 然后通过loss来减小sender和receiver加噪声数据分布的差异
3. 知乎有一个系列，介绍BFN的还不错
4. loss有两部分组成，$L_r$的物理意义。与VAE的相似性