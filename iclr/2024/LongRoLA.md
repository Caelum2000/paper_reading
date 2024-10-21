## Title: LongLoRA: Efficient Fine-tuning of Long-Context Large Language Models
1. 利用LoRA 微调 LLM, 使其能够有长文本的能力。例如微调前最长为L, 微调过后4L
2. 将4L切成4个L，然后分别做attention map
3. 相比直接用LoRA微调，时间复杂度较小，因为切分过，所以避免了平方的时间复杂度
4. 仅仅切分不够，还需要使不同段之间(group)交互起来，本文设计了一种位移的方法，使不同分段交互 Figure 3
5. 在Figure 3中，把self-attention的heads分更多组，给予不同的位移，能不能效果更好。因为这样交互的更多。