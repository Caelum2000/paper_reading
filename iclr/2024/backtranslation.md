## Self-Alignment with Instruction Backtranslation
1. 生成instruction数据用于微调LLM的工作
2. 分两个阶段：
   1. 首先爬取网上的数据然后根据文本生成instruction，文本内容就是用于回答instrcution, 由于是“生成问题”，所以叫backtranslation
   2. 过滤这些instruction pair得到高质量的pair
3. 以上用要fintune的LLM完成，所以叫self-xxx