### Information Transfer Across Clinical Tasks via Adaptive Parameter Optimisation
1. multitask优化
2. 主要的insight是：对于一个任务，往往只需要优化少数的权重，大部分参数变化不大，这证明对于一个task，神经网络是overparameterized
3. 在多任务时，保留重要的权重，引导不同任务权重不重叠，见Alg.1