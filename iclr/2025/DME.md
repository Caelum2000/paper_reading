### DYNAMIC MULTIMODAL EVALUATION WITH FLEXIBLE COMPLEXITY BY VISION-LANGUAGE BOOTSTRAPPING
1. 提出了一种新的multimodal llm的eval方法： Vision-Language Bootstrapping (VLB).
2. VLB是将网上的静态的作为eval的数据对text或image进行修改，从而生成新的数据，见Fig.3
3. VLB的好处包括不使eval数据和pretrain的大量数据重叠，可以控制eval的难度等