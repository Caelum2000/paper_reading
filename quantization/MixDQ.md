### MixDQ: Memory-Efficient Few-Step Text-to-Image Diffusion Models with Metric-Decoupled Mixed Precision Quantization
1. 提出了text2img模型量化的若干insights
2. 比如，clip embedding的第一个BOS token在范围上是outlier, 因此不进行量化
3. 提出SQNR（就是度量量化模型和精确模型的MSE差异）对生成质量和生成语义的解耦影响。并指出了影响质量和语义对应的层
4. Sec 3.3有一个整数规划，文章没太说清楚