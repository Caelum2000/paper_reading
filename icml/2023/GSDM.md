## Title: Graphically Structured Diffusion Models
1. 将图模型结构化的信息加入Diffusion这种生成模型
2. 算是神经符号主义的一种，文中也提到了这个词
3. 加结构信息的方法是更改 attention map ，在其中加入mask。没有边相连的节点就设置成mask。相当于把attention map当成邻接矩阵
4. 具体的细节和任务还需要学习概率图课程后细看