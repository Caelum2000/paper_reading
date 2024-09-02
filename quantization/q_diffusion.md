## Title: Q-Diffusion: Quantizing Diffusion Models
1. 指出了diffusion quantization的几个问题：
   1. 由于diffusion推理需要很多step，所以量化误差会累加
   2. 不同time step的激活值幅度不一样
2. 利用time step之间的数据修正量化过程，具体怎么修正没说
3. 单独拿出来shortcut连接来量化，因为shortcut的激活大小和其他的不一样
4. 论文有点不详细，具体看代码