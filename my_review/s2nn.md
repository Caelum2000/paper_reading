## S2NN: Self-Supervised Spiking Neural Networks with MixedLIF Neurons and Temporal Alignment

### Summary
This paper presents a self-supervised learning (SSL) framework tailored for spiking neural networks (SNNs), a class of biologically inspired neural networks that process information via binary spikes over time. Unlike traditional artificial neural networks, SNNs are inherently non-differentiable due to their discrete spiking mechanism, posing challenges for gradient-based optimization. To overcome this, the authors introduce MixedLIF neurons, which integrate the spiking behavior of traditional Leaky Integrate-and-Fire (LIF) neurons with a differentiable activation pathway, enabling effective training within an SSL paradigm. Additionally, a novel temporal contrastive loss is proposed to exploit the temporal dynamics of SNNs, aligning representations across time to enhance learning from unlabeled spiking data.
### Strengths And Weaknesses

- Strengths
    1. Investigating SSL with SNNs is a forward-thinking endeavor, merging biologically plausible models with cutting-edge machine learning techniques, potentially mirroring learning processes in the brain.
    2. Clarity of Presentation: The paper is well-organized and articulate, making its complex concepts approachable to readers.

- Weaknesses

    1. Results in Table 1 indicate only marginal improvements over baselines, casting doubt on the practical significance of the proposed framework.
    2. Differentiability Trade-Off: The differentiable Path B in MixedLIF neurons may conflict with the fundamental goal of SNNs to rely on binary spikes, potentially sacrificing advantages like energy efficiency and temporal sparsity.
    3. In Table 5, the comparison between LIF and MixedLIF neurons lacks an ablation study isolating Path B’s contribution, leaving uncertainty about whether the differentiable path disproportionately drives performance.
    4. The temporal contrastive loss might replicate the effects of simpler techniques, such as increasing batch size or data augmentation. A comparison of model parameters and computational costs with other methods in Table 1 is absent, hindering efficiency evaluation.
### Quality

good

### Clarity

good

### Significance

fair

### Questions

See weaknesses

### Limitations

No, I suggest that the author could include a limitation part after rebutall.

### Rating

3

### Confidence

3