# Title
> Brief summary of your review.
> Notes
    * Before you start entering your review, please read the slides at https://docs.google.com/presentation/d/1flN6vhWAEELQQ67s7rqqfR_JeQhp2cXwuD80m2qe3_g even if you are an experienced reviewer as we made significant changes this year.
    * Please remember that if a reviewer is flagged by an Area Chair as “highly irresponsible”, their paper submissions may be desk rejected per the discretion of the PCs.
    * Please remember that Large language models (LLMs) are NOT allowed to be used for writing the reviews nor the meta-reviews at any step. This is true for any LLM, whether you run it locally or use an API. This policy includes but is not restricted to:
    * You can’t ask an LLM to write content for you. The review needs to be based on your own judgment.
    * You can’t share substantial content from the paper or your review with an LLM. This means, for example, that you cannot use an LLM to translate a review.
    * You can use an LLM to do background research or to check short phrases for clarity. This includes using grammar checkers such as Grammarly.
    * The PCs will look actively for collusion rings. Reviewers caught at collaborating to manipulate the review process for mutual benefit will see their papers desk-rejected.

This work has potential contributions, but further clarification is needed regarding the novelty and the strength of the experiments.


## Paper Summary

> Summarize in your own words the paper, its key ideas, its contributions and their significance. This summary will help the AC and the authors understand the rest of your review and be confident that you understand the paper.

The article primarily focuses on improvements to the commonly used LIF neuron in Spiking Neural Networks (SNNs), proposing the DLIF neuron. In addition to considering the weighted input stimuli, the DLIF neuron also takes into account the interactions between different input stimuli. The authors use the cross-product of different input spike stimuli to represent this process. They demonstrate that DLIF neurons have a stronger expressive capability than LIF neurons, achieving tasks such as XOR classification and surpassing the performance of LIF neurons on other benchmarks.

## Paper Strengths

> List anything that you think could be of interest to readers and explain why. For example: What did you learn from the paper? Is there a key idea that could inspire others (remember that simple but powerful ideas can be more impactful than overly complicated architectures)? Does the paper present significant results that are likely of interest to people in the community?

1. This paper primarily focuses on improving the LIF model by introducing interaction terms between different input stimuli, thereby enhancing the expressive capability of individual neurons.  
2. The DLIF model aligns more closely with biological observations, where there is information interaction between dendrites, and a single neuron is capable of performing XOR classification tasks (as referenced in the study by reference 17).

## Major Weaknesses

> Describe here as carefully as possible the weaknesses that you think could justify a rejection. Major weaknesses include, but are not limited to: * The paper does not provide sufficient evidence to support the claims it makes. * The claims made by the paper are not novel. (you have to provide citations) * The claims made by the paper are not meaningful or of possible interest to the community. Remember that a submission is not required to compare to closed source papers per a recent PAMI-TC motion.

1. The article primarily proposes an interaction between different input stimuli through multiplication. However, from the perspective of deep learning, this mechanism is widely used in various models today. For example, in the case of learnable coefficients, the expression $\sum k_{ij} S_i(t) S_j(t)$ proposed in the article can be approximately reorganized into a cross-term form as $(\sum_i p_i S_i(t)) \cdot (\sum_j q_i S_j(t))$. This form is commonly used in attention mechanisms, where the query, key, and value (qkv) are passed through an MLP and then multiplied. Essentially, these mechanisms represent a learning process where different input stimuli interact through multiplication. From the perspectives of deep learning and pattern recognition, I think this method lacks a certain level of novelty.

2. From the perspective of computational neuroscience, the DLIF proposed in this paper is a more detailed imitation of biological neurons compared to the LIF model, aiming to validate the impact of this finer modeling approach. This is the primary contribution of the study from the viewpoint of computational neuroscience. However, the paper currently lacks some more "neuroscientific" experiments, such as simulating brain regions using DLIF or validating the similarity between DLIF and real neurons in performing cognitive tasks like classification by comparing neuronal behavior patterns.

3. Compared to the LIF neuron, the DLIF introduces an additional cross-term $\sum k_{ij} S_i S_j$, which adds extra computational complexity and learnable parameters. In the experimental section, the paper compares DLIF with other SNNs, but I am unsure whether this comparison was made under roughly the same computational load and parameter count. I recommend the authors can include additional experiments to clarify this.

## Minor Weaknesses

> Mention here the weaknesses that are easy to fix in a revision of the paper, such as occasional typographic errors and minor unclear points.

1. Some of the benchmarks used in the experimental section of this paper are relatively simple and old, such as the classification task on the CIFAR-10 dataset and the basic environment of DQN. I suggest that future work could include more advanced and modern experiments to demonstrate the effectiveness of DLIF, such as segmentation, image generation, and others.

## Overall Recommendation


* [ ] 5: accept
* [ ] 4: weak accept
* [x] 3: borderline
* [ ] 2: weak reject
* [ ] 1: reject


## Justification For Recommendation And Suggestions For Rebuttal

> Carefully balance in your answer the strengths and weaknesses to justify your recommendation. Explain to the authors what you would like to see clarified in order to change your opinion about the paper. You may request clarifications, additional illustrations, or small experiments that could be reasonably run within the rebuttal phase with academic resources. You should not request substantial additional experiments for the rebuttal, or penalize for lack of additional experiments. Please see the reviewer guidelines for more details.

To demonstrate the contribution and novelty of this paper, I think the authors need to fully address each issue, weakness, and question raised in the "major weaknesses" section and revise the paper accordingly. As for the additional experiments suggested in the "minor weaknesses" section, they may require significant effort during the rebuttal period, but I recommend that the authors complete as many of them as possible. Currently, the simple benchmarks are not sufficient to meet the CVPR threshold for the paper.


## Confidence Level


* [ ] 5: Expert - The reviewer is an authority in the specific subfield addressed by the paper. They are extremely confident in their evaluation and understanding of the work
* [ ] 4: High Confidence - The reviewer has strong expertise in the area. They are highly familiar with the relevant literature and can critically evaluate the paper.
* [x] 3: Moderate Confidence - The reviewer is reasonably knowledgeable about the topic. They understand the paper's methodology and results but may not be a leading expert in the specific subfield.
* [ ] 2: Low Confidence - The reviewer has some familiarity with the topic but does not have deep expertise. They might understand the paper but feel unsure about their evaluation.
* [ ] 1: Not Confident - The reviewer is unfamiliar with the topic, had difficulty understanding the paper, or is outside their area of expertise. Their judgment is likely unreliable.