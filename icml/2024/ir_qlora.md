## Accurate LoRA-Finetuning Quantization of LLMs via Information Retention
1. 指出了quant后的LLM LoRA效果差
2. 提出一种方法针对quant后llm进行LoRA
3. 注意看related work, 和Qloar什么区别
4. 放waiting list


### review
1. 更改了qloar中的quant方法，使normalfloat的分布更加均与，具体方法是对模型参数的权重进行平移缩放，使其更像标准正态分布
2. 魔改了lora把原来输入的x经过变形后加到了lora上