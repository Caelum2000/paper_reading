## Learning diffusion at lightspeed
1. 一种新的基于能量的类似diffusion的生成模型？
2. 放waiting list

### review
1. 指出diffsuion的SDE是基于最小化step之间的能量的
2. 通过学习step之间的能量，来学习diffusion，同时减小预测误差，见Eq.4
3. 将能量函数分解为势能，交互能，和内能来参数化，见Eq.11