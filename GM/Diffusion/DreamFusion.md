## Title: DreamFusion: Text-to-3D using 2D Diffusion
1. 通过diffusion的loss，设计了一种蒸馏方法。在Eq(1)中通过另一个模型(NeRF)学习图像x, 即$x=g(\theta)$
2. 在最终loss中忽略了一些项，得到了$L_{SDS}$ (Eq.3)