## SpikeLoRA: Power-Efficient Low-Rank Adaptation Based on Spiking Neural Network

### Summary

This paper proposes a PEFT method based on LoRA and the concept of spiking neural networks (SNN). Specifically, spike neurons (LIF) are inserted between the low-rank matrices used in LoRA, with the neural firing rate being employed for calculation. Additionally, the authors introduce a  initialization method for the LoRA low-rank matrices. The main claim is that SpikeLoRA enhances energy consumption efficiency during PEFT by leveraging the spiking dynamics.

### Strengths (optional)
### Weaknesses
1. The authors claim that SpikeLoRA is energy-efficient, but they do not provide details on how the FLOPs for SpikeLoRA are calculated or offer key insights to explain why the proposed method is more energy-efficient than ANN-based approaches. Intuitively, SpikeLoRA relies on the firing rate, which is a non-spike or non-binary variable. Additionally, SpikeLoRA appears to require multiple time steps, which may make it less efficient than ANN-based approaches.

2. I am concerned about the novelty and contribution of proposed initialization method. Theoretically, Eq. 14 suggests aligning the fine-tuned model with the pretrained model, but the "initialization method" appears to be an updating step toward this goal through SGD. 
### Questions (optional)
1. Regarding Weakness #1, I would like to understand why SpikeLoRA is considered energy-efficient. I hope the authors can clarify this with both theoretical proof and experimental validation (on real hardware, such as GPUs or other devices).

2. Please provide a further explanation of the novelty and contribution of the initialization method and how it differs from a simple one-step SGD used for model alignment.
### Reproducible
CREDIBLE
### Ethical
No
### Overall Assessment
Borderline reject
### Justify your score
Firstly, the main claim of this paper is that SpikeLoRA is energy-efficient, but intuitively, SpikeLoRA does not appear to be more energy-efficient than other LoRA-based approaches. The authors need to provide both theoretical proof and experimental validation (e.g., on NVIDIA GPUs or other hardwares) to support this claim. Secondly, the initialization method appears to be a simple SGD step aimed at aligning the pretrained model. The authors should clarify the novelty and contribution of the proposed method.
### Confident
Confident
### How well does this paper align with your expertise?
Knowledgeable