### ROGRESSIVE COMPRESSION WITH UNIVERSALLY QUANTIZED DIFFUSION MODELS
1. ddpm+ data compression
2. 方法是不同程度的noise对应不同的bit数，因此可以压缩。直观理解就是，噪声越大，信息越少，需要的bit越少
3. 用uniformal noise 代替 gaussian noise