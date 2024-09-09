## NEURAL FINE-TUNING SEARCH FOR FEW-SHOT LEARNING
1. 利用网络结构搜索(NAS)来做FSL
2. 采用的NAS方法基于SPOS. 就是先训练一个有所有结构的supernet，然后再进行选择，训练和选择分离
3. 分为meat-traininig 和 meta-test, meta-training会在一系列结构种选择适合该任务的结构，然后test。有点meta-learning的味道。见Fig.1