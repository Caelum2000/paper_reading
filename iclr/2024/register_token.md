## Title: VISION TRANSFORMERS NEED REGISTERS
1. 观察到基于ViT的模型的feature map有噪声点
2. 发现这些噪声点对应的模型输出token的norm都很大
3. 观察到这些噪声点往往出现在 backgroud上，这些位置携带语义信息很少
4. 猜想：这些噪声点携带全局的信息。通过实验，即用大norm和正常norm进行分类任务，确实观察到norm大的token分类效果好。因此验证了猜想
5. 结论：ViT容易把全局信息放到信息量较少backgroud patch上。从而照成了噪声点的现象
6. 提出一种方法解决这个问题：就是在image 打patch后加入额外的token,叫register token. 这样ViT就会把全局信息加到这些token上，从而norm大的噪声点就会消失