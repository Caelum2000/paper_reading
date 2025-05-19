### SAFETY ALIGNMENT SHOULD BE MADE MORE THAN JUST A FEW TOKENS DEEP
1. 贡献主要是三点：
   1. 指出目前safety alignment的问题在于其实只对齐了前面几个token的输出，从而诱导refuse的输出。例如sorry, i an't 或 Sure, i can 就可能导致不同的结果。说明本质是对齐了顺口溜的开头
   2. 提出一种data augmentation的方法，增强后的data前面是正常的，但后面却是拒绝输出的理由。这样的data虽然不合语言逻辑，但作者表明这样可以使safety alignment不指局限于前几个token
   3. 提出一种fine-tune的loss，可以保持前几个token的distribution变化较小，但后面被fine-tune的程度较大。
2. 如果对齐后的LLM只是通过前几个token来判断该问题的输出是否有害，那LLM更像一个分类器，binary的判断safety。让除了前几个token的后面的内容也拒绝输出其实是类似给“分类”找利用，类似于CoT的过程。也许可以有一个safety CoT?