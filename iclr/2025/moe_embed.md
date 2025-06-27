### YOUR MIXTURE-OF-EXPERTS LLM IS SECRETLY AN EMBEDDING MODEL FOR FREE
1. 主要是指出MoE中不同expert给出的概率也可能包含额外的特征或关于输入的信息
2. 提出MoEE, 将MoE 的expert probs作为单独的特征与hidden state的特征concat到一起