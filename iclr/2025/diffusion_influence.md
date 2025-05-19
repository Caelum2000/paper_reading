### INFLUENCE FUNCTIONS FOR SCALABLE DATA ATTRIBUTION IN DIFFUSION MODELS
1. 该工作将分类任务中的influence function adapt 到diffusion 领域
2. influence function是指在train data中去掉某一个数据，会有什么影响
3. 方法是研究如果反向优化带准备去掉数据的loss，最优值会有什么影响，见Eq.4
4. 对Eq.4进行了展开，并用一些方式高效地计算二阶项