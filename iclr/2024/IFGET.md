## LATENT TRAJECTORY LEARNING FOR LIMITED TIMES- TAMPS UNDER DISTRIBUTION SHIFT OVER TIME
1. 解决的是Evolving Domain Generalization（EDG）的问题。就是data domain的特征会随着时间不断变化演化，比如天气数据随全球气候变暖变化
2. EDG的数据集通常timestamps比较少，一个timestamp表示一个特定的数据domain比如在气候变暖进程下一个特定阶段的数据。
3. 主要是用SDE来插值不同timestamps之间的data，从而扩展总的timestamps, 需要在latent space进行
4. 具体数学细节和loss的细节没看，就是学SDE里一些项