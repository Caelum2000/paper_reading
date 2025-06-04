### Improved Distribution Matching Distillation for Fast Image Synthesis
1. 去掉了DMD种的regression loss
2. 使用了GAN loss，GAN的对象是student generator生成的图片和真实数据分布的图片
3. 开源，imagenet 7卡A100 两天, 开销有点高。cifar-10可能好一点？