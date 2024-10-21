## Video-LaVIT: Unified Video-Language Pre-training with Decoupled Visual-Motional Tokenization
1. 使LLM理解video，有生成功能
2. 怎么使LLM理解video？答:将video翻译成LLM的token然后autoregressive的利用LLM生成这些token。翻译方法是VQ-VAE
3. 怎么从生成video token生成video。使用的是vq-vae解码和diffusion
4. 这里用diffusion在于本工作对video clip选取了关键帧，然后diffusion用关键帧生成video
5. 本工作采用的是把key frame和motion信息变成token，这样可以减小计算复杂度
6. 需要训练的：tokenizer(vq-vae), LLM, diffusion