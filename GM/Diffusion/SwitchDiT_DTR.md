## DTR Title: Denoising Task Routing for Diffusion Models
1. 在diffusion的不同时间步，利用一个mask gate选择不同的channel，从而达到multi task的作用（不同时间步看作不同task）
2. mask gate是提前设置好的，不是学习的
3. 在SNN是否可以采用类似的思想，不同的SNN时间步是不同的task

## SwitchDiT Title: Switch Diffusion Transformer: Synergizing Denoising Tasks with Sparse Mixture-of-Experts
1. MoE 版本的 DiT
2. 设计了一个auxiliary loss, 好像是对其MoE的gating和一个预设的先验。具体实现看代码
3. 文中说auxiliry loss可以使EMA收敛，这是什么意思？