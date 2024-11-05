## Title: DreamFusion: Text-to-3D using 2D Diffusion
1. 通过diffusion的loss，设计了一种蒸馏方法。在Eq(1)中通过另一个模型(NeRF)学习图像x, 即$x=g(\theta)$
2. 在最终loss中忽略了一些项，得到了$L_{SDS}$ (Eq.3)
3. 本质上是借助text-to-image 的DDPM修正NeRF的参数，是NeRF渲染后的图像能够被训练好的DDPM去噪, 且应该符合text的condition。
4. 问题：怎么保证NeRF不同view之间的一致性？NeRF本身的模型结构可以保证这种一致性吗？