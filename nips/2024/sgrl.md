## Exploitation of a Latent Mechanism in Graph Contrastive Learning: Representation Scattering
1. 研究图上的对比学习
2. 放waiting list


### review
1. 研究的是图的对比学习。图对比学习就是在没用node的label下，自监督地学习到node的feature，当然，这个feature需要反映图的topology
2. 提出了representation scattering，就是使CL得到的feature满足在单位球上，且均匀分布
3. 指出representation scattering和其他图CL方法的联系，例如通过其他图CL方法学到的feature后验地满足均匀分布等
4. 整个流程Fig.3写的很清楚。注意是怎么使feature具有topology信息的，见Eq.5，是乘（k阶）邻接矩阵