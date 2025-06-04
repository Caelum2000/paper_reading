### Simple and Fast Distillation of Diffusion Models
1. 快速蒸馏
2. 不仅是对齐teacher和student之间某个时间步的gap，而是让student能累计时间步的误差，见Alg.1和Alg.2的对比
3. 收敛速度快，单卡A100仅需要8min？
4. 开源