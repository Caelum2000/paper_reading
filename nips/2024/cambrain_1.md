## Cambrian-1: A Fully Open, Vision-Centric Exploration of Multimodal LLMs
1. 提出MLLM要输入vision feature，而不是仅vision feature对其语言的embedding 然后输入LLM
2. 提出了一种新的vision encoder和MLLM之间的connector, 具体就是在不同尺度上提取visual feature. 作者认为这样能让下游的LLM更好的吸取vision的feature