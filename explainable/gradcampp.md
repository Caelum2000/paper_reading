## Grad-CAM++: Improved Visual Explanations for Deep Convolutional Networks
1. 改工作针对GradCam进行了微小的改进，使可视化效果看起来更好
2. GradCam就是对特征图的position加权重，权重等于Eq.3
3. GradCAM++就是在GradCAM的权重中加了apaptive factor, 见Eq.5， Fig.3
4. 这样干的效果是对阈值之上的position都有同样的权重，就会使热力图达到类似语义分割的效果，比较平均。见Fig.2