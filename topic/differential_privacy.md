## How to DP-fy ML: A Practical Guide to Machine Learning with Differential Privacy
### 来源：survey 论文

### DP的定义
1. 就是经过某个机制扰动，仍然可以大致符合原概率分布
2. 对任务进行DP的方法：对数据加DP，模型训练过程中加DP等


### DP-SGD
1. 在SGD的梯度中加噪声
2. 为什么DP-SGD符合DP的定义？证明过程没看
3. DP-SGD会牺牲模型性能，文中指出了一系列的挑战

### DP-SGD的实际应用
1. 怎么调参，如何解决性能下降等