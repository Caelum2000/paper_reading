## Universal Functional Regression with Neural Operator Flows
1. 使用neural operator 构建normalzing flow的生成模型
2. 将输入split，然后一部分用neural op学一个系数相乘，再加回去（见4.1 affine coupling）
3. 可以使用SNN，因为neural op没用在同胚的地方