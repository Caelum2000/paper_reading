## Title: 3D GENERATION ON IMAGENET
1. 之前的3D模型只能在单一类别的数据集上生成，这个工作可以在多类别比如ImageNet数据集上生成
2. 有一个camera generator, 能够生成相机参数，姿态角度等。
3. discriminator除了接受生成的3d信息还接受depth信息，有一个depth estimator