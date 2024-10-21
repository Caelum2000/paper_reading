## Title: Adversarial Example Does Good: Preventing Painting Imitation from Diffusion Models via Adversarial Examples
1. 利用对抗样本来使diffusion学不到某些图片
2. 对抗样本是通过图片微扰形成的
3. 可以用于保护某些画作或风格不被diffusion模仿，从而产生版权问题
4. 具体的应用场景是textual inversion。需要让图片作为condition的时候通过对抗样本使其不能很好的condition