## SAMformer: Unlocking the Potential of Transformers in Time Series Forecasting with Sharpness-Aware Minimization and Channel-Wise Attention
1. transformer做时间序列预测的工作
2. 分析了transformer在时间序列预测的loss 比较sharp。收敛到local minima的问题
3. 采用了sharp awareness的方法，具体是对模型参数进行扰动
4. 问题：为什么要用channel-wise attention