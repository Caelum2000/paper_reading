# Title: LINEAR MAPS, CONTRASTIVE OBJECTIVES: A PRINCIPLED STRATEGY FOR FMRI DECODING CONSISTENT ACROSS MODALITIES
# Summary*
*Briefly summarize the paper and its contributions. You can incorporate Markdown and Latex into your review. See https://openreview.net/faq.*

The paper argues that when decoding fMRI into the representation spaces of large foundation models, a simple linear mapping trained with a contrastive objective is consistently better than ridge regression and shallow MLPs. The authors evaluate three public datasets, and use retrieval in embedding space as the metric. A small architecture with subject-specific linear alignment followed by a linear projection yields Top-1 gains over ridge and also outperforms their non-linear MLP across all modalities. 

## Soundness*
*Please rate the paper in terms of its soundness. Are the central claims of the paper adequately supported with evidence? Are the experimental setup and research methodology sound?*


- [ ] 4: excellent
- [ ] 3: good
- [ ] 2: fair
- [x] 1: poor


## Presentation*
*Please rate the paper on the quality of the presentation. This should take into account the writing style and clarity, presentation of figures and diagrams, as well as contextualization relative to prior work.*

- [ ] 4: excellent
- [ ] 3: good
- [x] 2: fair
- [ ] 1: poor

## Contribution*
*Please rate the quality of the overall contribution this paper makes to the research area being  studied. Are the questions being asked important? Does the paper bring a significant originality of ideas and/or execution? Are the results valuable to share with the broader ICLR community?*

- [ ] 4: excellent
- [ ] 3: good
- [x] 2: fair
- [ ] 1: poor


## Strengths*
*A substantive assessment of the strengths of the paper, touching on each of the following dimensions: originality, quality, clarity, and significance. We encourage reviewers to be broad in their definitions of originality and significance. For example, originality may arise from a new definition or problem formulation, creative combinations of existing ideas, application to a new domain, or removing limitations from prior results.*

The paper’s key strength is its evidence that a simple linear mapping is adequate for aligning fMRI signals with semantically rich embedding spaces (e.g., from multimodal foundation models). This is a surprising and consequential observation, suggesting that the geometry of brain-recorded activity admits an approximately linear relationship to these representations, thereby refining our understanding of both fMRI signal structure and neural encoding at the population level.

## Weaknesses*
*A substantive assessment of the weaknesses of the paper. Focus on constructive and actionable insights on how the work could improve towards its stated goals. Be specific, avoid generic remarks. For example, if you believe the contribution lacks novelty, provide references and an explanation as evidence; if you believe experiments are insufficient, explain why and exactly what is missing, etc.*


Although the conclusion—that an efficient linear mapping suffices for fMRI decoding—is intriguing, the experimental design supporting this claim appears insufficiently rigorous:

1. The paper compares ridge regression (trained with an MSE objective and L2 regularization ?) to the proposed linear model trained with a contrastive (InfoNCE-style) objective. Because the target embedding (e.g., CLIP) itself is learned with a contrastive loss, this comparison is not fair: one would expect a method trained with a geometry-aligned contrastive loss to outperform MSE by construction. 

2. The paper states that an MLP underperforms the linear model (Table 1), yet Table 2 shows that **Identity** activation yields the best MLP performance. Theoretically, an MLP with identity activations collapses to a linear map; with sufficient training and comparable regularization, it should match (or closely approach) the linear model. So does the comparsion of MLP with identity activation and linear model make sense?

3. The proposed linear model includes a subject-specific adjustment matrix (A_k). It is unclear whether the MLP baseline incorporates an analogous adjustment . The paper should document these details (main text or appendix).

I am willing to increase my score if the authors address the issues above.

## Questions*
*Please list up and carefully describe any questions and suggestions for the authors. Think of the things where a response from the author can change your opinion, clarify a confusion or address a limitation. This is important for a productive rebuttal and discussion phase with the authors.*

1. Please according to the soundness issues in Weaknesses part
2. It is recommend that the author could explain more why linear model is better than other more complex methods.


## Rating*
*Please provide an "overall score" for this submission.*


- [ ] 0: strong reject.
- [ ] 2: reject, not good enough
- [x] 4: marginally below the acceptance threshold. But would not mind if paper is accepted
- [ ] 6: marginally above the acceptance threshold. But would not mind if paper is rejected
- [ ] 8: accept, good paper (poster)
- [ ] 10: strong accept, should be highlighted at the conference as spotlight or oral.


## Confidence*
*Please provide a "confidence score" for your assessment of this submission to indicate how confident you are in your evaluation.*


- [ ] 1: You are unable to assess this paper and have alerted the ACs to seek an opinion from different reviewers.
- [ ] 2: You are willing to defend your assessment, but it is quite likely that you did not understand the central parts of the submission or that you are unfamiliar with some pieces of related work. Math/other details were not carefully checked.
- [x] 3: You are fairly confident in your assessment. It is possible that you did not understand some parts of the submission or that you are unfamiliar with some pieces of related work. Math/other details were not carefully checked.
- [ ] 4: You are confident in your assessment, but not absolutely certain. It is unlikely, but not impossible, that you did not understand some parts of the submission or that you are unfamiliar with some pieces of related work.
- [ ] 5: You are absolutely certain about your assessment. You are very familiar with the related work and checked the math/other details carefully.