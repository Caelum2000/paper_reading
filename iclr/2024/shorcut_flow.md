### ONE STEP DIFFUSION VIA SHORTCUT MODELS
1. 基于flow model提出shortcut model，就是一步相当于走flow model的很多步。
2. 具体图解见Fig.3。以及在loss中的s_target项，其实就是让两项vector合并成一项(Eq.4, Eq.5)
3. 使用JAX在TPU上训练，目前不太能access