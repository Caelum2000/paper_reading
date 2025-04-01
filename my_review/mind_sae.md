## MindSAE: A Unified Multimodal Alignment Framework for Zero-Shot M/EEG-Based Visual Decoding

## 1. Please briefly summarize the main claims/contributions of the paper in your own words.
This work primarily adopts a CLIP-like method for EEG stimulus image retrieval and stimulus category classification. The proposed approach uses a trainable EEG signal encoder to align the encoded representation with CLIP's image and text representations. For the text representation, the authors utilize MLLM to generate both coarse and fine-grained text descriptions, enhancing the representation of features at various levels.

## 2. What are the main strengths of the paper? 
1. The pipeline learns a unified representation for both tasks, enabling simultaneous zero-shot M/EEG-based visual stimulus retrieval and classification.  
2. MLLM is used to generate both coarse and fine-grained text descriptions, improving the alignment's upper bound.

## 3. What are the weaknesses of the paper? 
1. The concept of MindSAE is largely from the CLIP pipeline, with the proposed method training only an encoder to align with CLIP features.  
2. Using both coarse and fine-grained features to model EEG or fMRI signals is not a fresh approach. Many other studies have applied this concept to more complex tasks, such as image or text reconstruction.  
3. Given the points above, I think the main issue with this work is that its contribution and novelty are relatively limited.

## 4. Please carefully list the questions that you would like the authors to answer during the author-feedback period. 
See Section 3

[Your response here - 6000 characters left]

## 5. Are the results of this paper easily reproducible?
Choose one of the following:
- CONVINCING: I am convinced that the obtained results can be reproduced, possibly with some effort. Key resources (e.g., proofs, code, data) are already available, will be made available upon acceptance, or good reasons as to why they are not (e.g., proprietary data or code) are reported in the paper. Key details (e.g., proofs, experimental setup) are sufficiently well described.


## 6. Independent of your judgement of the quality of the work, are there any ethical concerns with regard to responsible research or potential negative societal impacts of this submission that must be considered by IJCAI 2025 before the paper can be accepted? 

- No ethical concern

## 7. Overall Assessment *
*(visible to authors after notification, visible to other reviewers, visible to meta-reviewers, visible to senior meta-reviewers)*


- Borderline Reject: Marginally below the acceptance threshold. The paper has merits but there are key weaknesses. It would benefit from another revision. Can be rejected. But having it in the program would not be that bad. Please use sparingly.



## 9. How confident are you in your evaluation? *

- Confident: I tried to check the key points in the paper. It is unlikely, though conceivable, 

## 10. How well does this paper align with your expertise? *

- Knowledgeable: This paper has overlaps with my core research focus and I am knowledgeable about most of the topics covered by the paper.


## 11. Confidential comments to SPC, AC, SAC and Program Chairs
N/A