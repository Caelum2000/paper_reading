## Summary*
> Briefly summarize the paper (including the main findings, main results, main algorithmic/conceptual ideas, etc. that the paper claims to contribute). This summary should not be used to critique the paper. A well-written summary should not be disputed by the authors of the paper or other readers.

This paper proposes **LaVCa**, a classify and caption pipeline designed for brain voxel analysis. **LaVCa** utilizes a voxel encoder to align voxel representations with image **CLIP** embeddings. It then employs a contrastive approach (which is used in CLIP), to classify the voxel data. After identifying the optimal image from a dataset based on the classification results, **LaVCa** leverages a **MLLM** to generate a caption for the selected image.

## Claims And Evidence*
>Are the claims made in the submission supported by clear and convincing evidence? If not, which claims are problematic and why?

Yes


## Methods And Evaluation Criteria
> Do proposed methods and/or evaluation criteria (e.g., benchmark datasets) make sense for the problem or application at hand?

Yes

## Theoretical Claims*
> Did you check the correctness of any proofs for theoretical claims? Please specify which ones, and discuss any issues.

Seems like no theoretical claims or proof in this paper. 

## Experimental Designs Or Analyses*
> Did you check the soundness/validity of any experimental designs or analyses? Please specify which ones, and discuss any issues.

No issuses


## Supplementary Material*
> Did you review the supplementary material? Which parts?

Yes, I have skimmed through the supplementary material.


## Relation To Broader Scientific Literature*
> How are the key contributions of the paper related to the broader scientific literature? Be specific in terms of prior related findings/results/ideas/etc.

I believe this work may inspire us to leverage pretrained models to address previously challenging problems. This approach has recently gained significant traction, not only in scientific fields but also in areas such as art, writing, and beyond.


## Essential References Not Discussed*
> Are there related works that are essential to understanding the (context for) key contributions of the paper, but are not currently cited/discussed in the paper? Be specific in terms of prior related findings/results/ideas/etc. (Example: "The key contribution is a linear-time algorithm, and only cites a quadratic-time algorithm for the same problem as prior work, but there was also an O(n log n) time algorithm for this problem discovered last year, namely Algorithm 3 from [ABC'24] published in ICML 2024.")

No, to my best knowledge.

## Familiarity With Literature*
> How well-versed are you with the literature related to this paper? (Examples: "I keep up with the literature in this area."; "I am only familiar with a few key papers in this area, namely [ABC'02], [DEF'04], and [GHI'05].") Note: Your response to this item will not be visible to authors. Please also see reviewer instructions regarding concurrent work.

I have been involved in research on generating human-friendly signals (such as images) from brain signals. However, I am not specifically focused on voxel classification and captioning in this area.


## Other Strengths And Weaknesses*
> Enter any comments on other strengths and weaknesses of the paper, such as those concerning originality, significance, and clarity. We encourage you to be open-minded in terms of potential strengths. For example, originality may arise from creative combinations of existing ideas, removing restrictive assumptions from prior theoretical results, or application to a real-world use case (particularly for application-driven ML papers, indicated in the flag above and described in the Reviewer Instructions).

- **Strength**:  
  - The key contribution of this work is leveraging the capabilities of large multimodal models (MLLMs) to generate captions based on voxel information. In contrast, previous approaches typically required fine-tuning or training caption models to accomplish this task.

- **Weakness**:
  - The contribution and novelty of this work are relatively limited, as it primarily involves incorporating a large model to caption the selected images.  
  - Although the generated captions outperform those of previous works, this improvement mainly stems from the capabilities of pretrained MLLMs rather than novel methodological advancements.



## Other Comments Or Suggestions*
> If you have any other comments or suggestions (e.g., a list of typos), please write them here.

No additional comments


## Questions For Authors*
> If you have any important questions for the authors, please carefully formulate them here. Please reserve your questions for cases where the response would likely change your evaluation of the paper, clarify a point in the paper that you found confusing, or address a critical limitation you identified. Please number your questions so authors can easily refer to them in the response, and explain how possible responses would change your evaluation of the paper.

Please review the weaknesses section. I believe the authors need to further clarify the novelty and contribution of this work.




## Overall Recommendation*

- [] 5: Strong accept
- [] 4: Accept
- [] 3: Weak accept (i.e., leaning towards accept, but could also be rejected)
- [x] 2: Weak reject (i.e., leaning towards reject, but could also be accepted)
- [] 1: Reject