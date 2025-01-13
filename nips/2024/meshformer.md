## MeshFormer: High-Quality Mesh Generation with 3D-Guided Reconstruction Model
1. 根据不同角度输入的图像重建3d物体
2. 先用diffusion来估计RGB中类似深度图的东西，文中说是normal map
3. 再使用voxel来重建3d物体，重建方式是用一个voxel former，具体不知道是什么