### SCALING AND EVALUATING SPARSE AUTOENCODERS
1. 探究scaling sparse autoencoder对系列结果的影响
2. 采用了k-parse autoencoder, 就是仅选取latent中TopK的几个激活。这样的好处相当于加了无穷范数约束，，见Sec 2.3
3. 是否可以用snn的思想代替上述的TopK, 改变如阈值等来控制激活的latent的数目
4. 放到relevant，但该工作训练规模较大，作者在甚至写了专用的核函数