## Genie: Generative Interactive Environments
1. 可以交互的video生成模型，可以被认为是world model
2. 与ICLR2024 Learning Interactive Real-World Simulators 很类似，都是google deepmind
3. 采用的是VQ-VAE的范式，而ICLR那篇是diffusion范式
4. 需要和iclr那篇对比研究一下细节


### review
1. 和Learning Interactive Real-World Simulators相比，使用的是vq-vae, 而那一篇是diffusion。并且考虑到了frame之间的action编码。但是场景比较有限，action只能是codebook中的固定action
2. 具有一个action encoder 提取frame之间action的embedding，还有一个video tokenizer, 用于把video打成vq-vae的vector
3. 然后根据action和video token计算下一个token