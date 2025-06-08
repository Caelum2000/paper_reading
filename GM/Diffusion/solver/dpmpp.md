### DPM-SOLVER++: FAST SOLVER FOR GUIDED SAMPLING OF DIFFUSION PROBABILISTIC MODELS
1. 针对DPM-solver进行改进。主要motivation在于发现基于high-order的diffusion reverse solver对于guidance的表现很差，作者认为主要是guidance增大了score的模长，从而high-order不收敛
2. 提出了另一种方法去估计$x_{\theta}$(数据本身)，而不是噪声$\epsilon_{\theta}$.证明这样更容易收敛
3. 其他和DPM-solver差不多
4. 设计了多步的DPM-solver，见Alg.2. 是否可以和replay结合？