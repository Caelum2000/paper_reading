## The Stronger the Diffusion Model, the Easier the Backdoor: Data Poisoning to Induce Copyright Breaches Without Adjusting Finetuning Pipeline
1. 研究怎么让stablediffusion生成会侵权的作品
2. 具体方式是生成一系列posion的数据，然后给SD训练
3. posion data需要近似有版权的数据，但不完全一样，这样有欺骗性。具体生成方法见Fig.1