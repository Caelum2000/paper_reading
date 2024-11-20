## Chain of Code: Reasoning with a Language Model-Augmented Code Emulator
1. 类似CoT的idea，该工作使LLM将一个问题转化为写代码问题，并生成代码
2. 生成的代码需要另一个解释器/编译器/sub-LM去执行得到结果。这一步可能比较消耗时间和计算资源