## Title: AWQ: Activation-aware Weight Quantization for LLM Compression and Acceleration
1. 有些weight比较重要，通过一些方法可以选出重要的weight
2. 通过scale这些weight可以减小量化误差，见Eq.2 Eq.3
3. scale factor可以搜索，见Eq.4