## Title: Learning Interactive Real-World Simulators
1. 利用video diffusion 训练了一个世界模型
2. 给定一张图片，Unsim可以根据输入的指令生成基于图片的视频。例如，移动鼠标等
3. 可以用在RL, VLM等领域
4. 使用了condition diffsuion，将之前生成的frames和text-action 条件输入diffusion。但这里frames的condition方法好像是将已经生成好的frames和噪声concat到一起，使用的是video diffusion框架