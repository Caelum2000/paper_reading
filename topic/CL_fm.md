## Continual Learning for Foundation Models
### 来源：基金需要调研 


### parameter efficient fine tune (PEFT) + CL
1. 采用微调的方式使模型获得新知识
2. Continual Learning with Low Rank Adaptation 根据不同domain的数据训练了不同LoRA，然后选择 

### CL + Instruction Tuning
1. 利用instruction tuning的方式使LLm能够根据instruct来进行对应的任务。比如让ta翻译或者文章润色
2. instruction在这里充当task的软标签？
3. 还需要其他方式进行CL，例如回放，因为instruct本身只是标签
4. Fine-tuned Language Models are Continual Learners 基于回放
5. SwitchCIT: Switching for Continual Instruction Tuning of Large Language Models 基于LoRA


### Continual Pretraining
1. 主要是解决在LLM pretrain的时候，会对大量不同domain的数据遗忘的问题
2. Examining Forgetting in Continual Pre-training of Aligned Large Language Models 研究LLM预训练遗忘已经一些应对方法
3. Continual Pre-Training of Large Language Models: How to (re)warm your model? 研究怎么通过warm up解决LLM 预训练阶段的遗忘问题

### Knowledge Distillation
1. 在训练k个任务时，保留k-1模型的能力
2. 具体方法就是在loss分两部分：k task本身的loss+ 与前面teacher模型表征对齐的loss
3. Selective Dual-Teacher Knowledge Transfer for Continual Learning on Vision-Language Models 通过学习一个权重，选择性地蒸馏基础大模型或者在前面一系列任务上微调的模型

### Modular Architectures
1. MoE
2. Adapter

### Prompt Tuning + CL
1. prompt在这里是可以学习的一个vector，和LLM那个不一样
2. 通过可学习的prompt，作为标签或者condition，从而给模型指明是哪一个task
3. Learning to Prompt for Continual Learning (L2P) 该框架的提出者
4. Introducing Language Guidance in Prompt-based Continual Learning 使用语言encoder指导prompt pool的分布
