### CONTEXT-PARAMETRIC INVERSION: WHY INSTRUCTION FINETUNING CAN WORSEN哦CONTEXT RELIANCE
1. 主要是研究如果用户对llm给出的context和llm本身学习到的知识矛盾时,会产生conflict的现象
2. 主要发现是在instruction tuning阶段，这种conflict会先下降，再上升
3. 先下降是因为instruction tuning 本事就是要llm去理解上下文，上升的原因在于随着训练数据的增加，数据的bias影响增大