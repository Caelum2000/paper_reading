## Candidate Pseudolabel Learning: Enhancing Vision-Language Models by Prompt Tuning with Unlabeled Data
1. 使用unlabel的data去finetune VLM
2. 具体没看，放waiting list


### review
1. 对一个unlabel的数据生成很多candidate labels, 然后再用多label的loss进行训练
2. 生成方法是用VLM生成概率（如何生成概率，prompt是什么），然后用分位数选其中的一些label作为candidate