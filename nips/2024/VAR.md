## Visual Autoregressive Modeling: Scalable Image Generation via Next-Scale Prediction
1. 设计了一个multi scale的VQ-VAE，然后利用自回归来进行图像生成
2. 自回归模型是next scale prediction。就是用已知的scale经过vq-vae后的code预测下一个scale的code。分辨率不断增加