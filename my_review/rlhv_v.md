# Safe RLHF-V: Safe Reinforcement Learning from Multi-modal Human Feedback
## Summary*
*Briefly summarize the paper and its contributions. This is not the place to critique the paper; the authors should generally agree with a well-written summary. This is also not the place to paste the abstract—please provide the summary in your own understanding after reading.*

> comments here.

This article aims to investigate safety alignment fine-tuning techniques based on multimodal large models. Previous fine-tuning approaches based on Reinforcement Learning from Human Feedback (RLHF) have typically been applied to language-only large language models, with limited application to vision-language models, thus this paper partially addresses this gap. The contributions of this paper are threefold: first, it proposes a dataset for multimodal RLHF alignment; second, it designs a defense system against harmful outputs for multimodal large models; and third, it improves safe RLHF by dynamically updating the Lagrange coefficients in constrained optimization.



## Strengths And Weaknesses*
*Please provide a thorough assessment of the strengths and weaknesses of the paper. A good mental framing for strengths and weaknesses is to think of reasons you might accept or reject the paper. Please touch on the following dimensions: Quality, Clarity, Significance, and Originality. For more information, please see the NeurIPS 2025 Reviewer Guidelines (https://neurips.cc/Conferences/2025/ReviewerGuidelines). You can incorporate Markdown and LaTeX into your review. See https://openreview.net/faq.*

> comments here. 
### Strength:
1. The topic of multimodal alignment and the balance between its safety and usability has been underexplored and is of significant importance.

2. The workload of this paper is substantial, and its results are comprehensive. Centered on the theme of multimodal alignment, it not only proposes a new dataset (along with a data collection methodology) but also designs a harmful output detection system and introduces algorithmic innovations for safe RLHF. Overall, the content is systematic and robust.

### Weaknesses:
1. This work improves the algorithm based on safe RLHF, resulting in safe RLHF-V. However, the novelty appears limited. The authors dynamically update the Lagrange coefficient in Equations 7 and 8, increasing the coefficient to impose greater penalties when the cost is high, and decreasing it otherwise. For such constrained optimization problems, a common approach is to fix the value of λ (i.e., treating it as a hyperparameter for the penalty term, such as in L1-based weight sparsity). The contribution of this algorithm seems to lie solely in the dynamic adjustment of this coefficient.

2. There are some minor issues, such as the lack of explanation for the meanings of the variables in Equations 7 and 8. It is recommended to review the readability of the entire text and include additional details in the main body.



## Quality*
*Based on what you discussed in "Strengths and Weaknesses", please assign the paper a numerical rating on the following scale to indicate the quality of the work.*

- [ ] 4: excellent
- [x] 3: good
- [ ] 2: fair
- [ ] 1: poor


## Clarity*
*Based on what you discussed in "Strengths and Weaknesses", please assign the paper a numerical rating on the following scale to indicate the clarity of the paper.*

- [ ] 4: excellent
- [ ] 3: good
- [x] 2: fair
- [ ] 1: poor


## Significance*
*Based on what you discussed in "Strengths and Weaknesses", please assign the paper a numerical rating on the following scale to indicate the significance of the paper.*

- [ ] 4: excellent
- [x] 3: good
- [ ] 2: fair
- [ ] 1: poor


## Originality*
*Based on what you discussed in "Strengths and Weaknesses", please assign the paper a numerical rating on the following scale to indicate the originality of the paper.*

- [ ] 4: excellent
- [x] 3: good
- [ ] 2: fair
- [ ] 1: poor


## Questions*
*Please list up and carefully describe questions and suggestions for the authors, which should focus on key points (ideally around 3–5) that are actionable with clear guidance. Think of the things where a response from the author can change your opinion, clarify a confusion or address a limitation. You are strongly encouraged to state the clear criteria under which your evaluation score could increase or decrease. This can be very important for a productive rebuttal and discussion phase with the authors.*

> comments here. 

Please see weaknesses. I will increase my rating if the authors can demonstrate the novelty of the RLHF-V algorithm.


## Limitations*
*Have the authors adequately addressed the limitations and potential negative societal impact of their work? If so, simply leave “yes”; if not, please include constructive suggestions for improvement. In general, authors should be rewarded rather than punished for being up front about the limitations of their work and any potential negative societal impact. You are encouraged to think through whether any critical points are missing and provide these as feedback for the authors.*

> comments here. 

It is recommended that the authors include a limitations section in the main text to provide a more detailed description of the study's limitations.


## Rating*

- [ ] 6: Strong Accept: Technically flawless paper with groundbreaking impact on one or more areas of AI, with exceptionally strong evaluation, reproducibility, and resources, and no unaddressed ethical considerations.
- [ ] 5: Accept: Technically solid paper, with high impact on at least one sub-area of AI or moderate-to-high impact on more than one area of AI, with good-to-excellent evaluation, resources, reproducibility, and no unaddressed ethical considerations.
- [x] 4: Borderline accept: Technically solid paper where reasons to accept outweigh reasons to reject, e.g., limited evaluation. Please use sparingly.
- [ ] 3: Borderline reject: Technically solid paper where reasons to reject, e.g., limited evaluation, outweigh reasons to accept, e.g., good evaluation. Please use sparingly.
- [ ] 2: Reject: For instance, a paper with technical flaws, weak evaluation, inadequate reproducibility and incompletely addressed ethical considerations.
- [ ] 1: Strong Reject: For instance, a paper with well-known results or unaddressed ethical considerations.


## Confidence*

- [ ] 5: You are absolutely certain about your assessment. You are very familiar with the related work and checked the math/other details carefully.
- [ ] 4: You are confident in your assessment, but not absolutely certain. It is unlikely, but not impossible, that you did not understand some parts of the submission or that you are unfamiliar with some pieces of related work.
- [ ] 3: You are fairly confident in your assessment. It is possible that you did not understand some parts of the submission or that you are unfamiliar with some pieces of related work. Math/other details were not carefully checked.
- [x] 2: You are willing to defend your assessment, but it is quite likely that you did not understand the central parts of the submission or that you are unfamiliar with some pieces of related work. Math/other details were not carefully checked.
- [ ] 1: Your assessment is an educated guess. The submission is not in your area or the submission was difficult to understand. Math/other details were not carefully checked.




