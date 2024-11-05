## Robust CLIP: Unsupervised Adversarial Fine-Tuning of Vision Embeddings for Robust Large Vision-Language Models

1. 解决CLIP被对抗攻击的问题
2. 方法是优化Eq.3, 就是使CLIP对于有扰动的输入能稳定
3. Eq.3中的max可以通过projected gradient descent实现，这个具体怎么实现不懂 