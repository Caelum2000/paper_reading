## GradSafe: Detecting Jailbreak Prompts for LLMs via Safety-Critical Gradient Analysis
1. 通过分析promopt的梯度来判断这个prompt是否有害
2. 梯度是通过比较LLM的回答和"sure"的loss来计算的
3. 可以从参数中选取一些和prompt safety相关的参数，这些参数对prompt的safety比较敏感
4. 分为GradSafe-Zero和GradSafe-Adapt两个不同的版本。GradSafe-Zero通过余弦相似度判断是否safe，GradSafe-Adapt通一个回归分类器判断