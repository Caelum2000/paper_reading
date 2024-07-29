## Title: Cameras as Rays: Pose Estimation via Ray Diffusion
1. 用diffusion做相机姿态估计。采用每个patch上射线的方法估计相机位置
2. 把图片特征，位置和方向输入DDPM。推理的时候把位置和方向换成噪声