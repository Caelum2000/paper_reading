# TS-LIF: A TEMPORAL SEGMENT SPIKING NEURONNETWORK FOR TIME SERIES FORECASTING

## Summary
This article improves the dynamical characteristics of the LIF neuron and proposes a TS-LIF model for time series forecasting, incorporating interactions between dendrites and soma. The authors analyze the robustness and functionality of the improved dynamical system's different components and validate through experiments that TS-LIF outperforms the standard LIF on time series prediction benchmarks.

## Soundness
3:good

## Presentation
3:good

## Contribution
2:fair

## Strengths
1. The analysis of the improved model is quite thorough.  
2. Experiments demonstrate that it outperforms previous SNN-based methods.  
3. The writing is clear and easy to understand.

## Weaknesses
The main issue with this article is the somewhat **unclear connection between the motivation and contributions**. I believe the authors need to clarify their motivation for using a spiking model for time series tasks. 

**If the goal of using a spiking model is to achieve better performance, the following points should be addressed:**

1. If the spiking model is used to improve performance, it should be compared with the latest state-of-the-art methods, such as [1] and [2].
2. In the introduction, it states, "In contrast, SNNs, with their event-driven and sparse computational architecture, can offer a more efficient solution, particularly for applications that involve sparse temporal events and demand low energy consumption." If the motivation for using a spiking model is to achieve low energy consumption, then additional experiments on hardware platforms should be provided to verify the model's energy efficiency, including specific tests on platforms like FPGA, GPU, and CPU to support this claim.
3. The authors improved the model by introducing input stimuli into the soma, achieving a symmetric dynamical form. While this improvement indeed enhances performance, it also introduces additional computational overhead. I believe it would be beneficial to compare this model to others in terms of parameter count, training time, and FLOPs to illustrate the advantages of using a spiking model.

**In the abstract, the authors mention that the spiking model is a biologically inspired neural network. If the purpose of this work is to validate the biological plausibility of this approach (or if the motivation is computational neuroscience rather than merely solving an engineering problem), then I believe the following points should be further addressed.**

1. In the proposed dynamic form where input stimuli are added to the soma rather than only to the dendrites, is there evidence that this mechanism is employed in the brain **for similar time series forecasting processes**?
2. Can dynamics or data similar to TS-LIF be observed in the biological brain, thereby validating that TS-LIF indeed simulates brain mechanisms?
3. It is suggested that the authors theoretically connect "shortcuts in soma" to analogous time series prediction processes in the brain, such as through predictive coding, active inference, etc. (This is optional, as it is challenging, but it would greatly enhance the contribution of the paper.)

[1] Lin S, Lin W, Wu W, et al. SparseTSF: Modeling Long-term Time Series Forecasting with 1k Parameters[J]. arXiv preprint arXiv:2405.00946, 2024.

[2] Ilbert R, Odonnat A, Feofanov V, et al. Unlocking the potential of transformers in time series forecasting with sharpness-aware minimization and channel-wise attention[J]. arXiv preprint arXiv:2402.10198, 2024.

## Questions

Please see weaknesses.

## Flag For Ethics Review
No ethics review needed.

## Rating
5:marginally below the acceptance threshold

## Confidence
4: You are confident in your assessment, but not absolutely certain. It is unlikely, but not impossible, that you did not understand some parts of the submission or that you are unfamiliar with some pieces of related work.