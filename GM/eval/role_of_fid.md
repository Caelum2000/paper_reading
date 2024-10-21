## Title: The Role of ImageNet Classes in Fr\'echet Inception Distance

1.  由于FID是用 ImageNet-pretrained inception-v3 计算的，因此生成图像中的 ImageNet 特征可能会影响FID
2.  通过Gard-CAM 显示，图像中的具有imagenet类的位置对FID有更重要的影响
3.  更具有imagenet 类别特征的图片FID会更好
4.  对于imagenet pretrained的discriminator会有更好的FID，但这是作弊，其实质量不一定好(可以调FID用)