## Summary*
> Briefly summarize the paper (including the main findings, main results, main algorithmic/conceptual ideas, etc. that the paper claims to contribute). This summary should not be used to critique the paper. A well-written summary should not be disputed by the authors of the paper or other readers.

The article proposes a neural network that is constructed using a local loss and asymmetric weights in the forward and backward passes. The author introduces three criteria for biological plausibility that the neural network should satisfy and demonstrates that the proposed DLL meets these criteria. The author also shows through experiments that DLL outperforms other non-traditional BP networks.

## Claims And Evidence*
>Are the claims made in the submission supported by clear and convincing evidence? If not, which claims are problematic and why?

Yes


## Methods And Evaluation Criteria
> Do proposed methods and/or evaluation criteria (e.g., benchmark datasets) make sense for the problem or application at hand?

Yes


## Theoretical Claims*
> Did you check the correctness of any proofs for theoretical claims? Please specify which ones, and discuss any issues.

Yes, I checked the math and didn't find any obvious issues.


## Experimental Designs Or Analyses*
> Did you check the soundness/validity of any experimental designs or analyses? Please specify which ones, and discuss any issues.

The author demonstrates the advantage of DLL over other non-traditional BP methods through experiments, but I think more ablation studies need to be added to prove that the three design criteria for biological plausibility of DLL contribute to improving the model's performance. This will enhance the soundness of this work.


## Supplementary Material*
> Did you review the supplementary material? Which parts?

Yes, Appidx A



## Relation To Broader Scientific Literature*
> How are the key contributions of the paper related to the broader scientific literature? Be specific in terms of prior related findings/results/ideas/etc.

I think the research in this paper is related to brain-inspired computation and computational neuroscience.


## Essential References Not Discussed*
> Are there related works that are essential to understanding the (context for) key contributions of the paper, but are not currently cited/discussed in the paper? Be specific in terms of prior related findings/results/ideas/etc. (Example: "The key contribution is a linear-time algorithm, and only cites a quadratic-time algorithm for the same problem as prior work, but there was also an O(n log n) time algorithm for this problem discovered last year, namely Algorithm 3 from [ABC'24] published in ICML 2024.")

No.


## Familiarity With Literature*
> How well-versed are you with the literature related to this paper? (Examples: "I keep up with the literature in this area."; "I am only familiar with a few key papers in this area, namely [ABC'02], [DEF'04], and [GHI'05].") Note: Your response to this item will not be visible to authors. Please also see reviewer instructions regarding concurrent work.

I am familiar with some papers in related fields, such as the forward-forward and predictive coding compared in the article, but I haven't delved deeply into this direction.



## Other Strengths And Weaknesses*
> Enter any comments on other strengths and weaknesses of the paper, such as those concerning originality, significance, and clarity. We encourage you to be open-minded in terms of potential strengths. For example, originality may arise from creative combinations of existing ideas, removing restrictive assumptions from prior theoretical results, or application to a real-world use case (particularly for application-driven ML papers, indicated in the flag above and described in the Reviewer Instructions).

* **Strengths**
    - The article summarizes the characteristics of some non-traditional BP learning methods, extracts three criteria, and designs DLL based on them. Experimental results demonstrate that DLL can outperform previous similar methods.
    - In today's world where SGD is widely used, exploring new learning methods is refreshing and can increase attention to learning approaches within the field.

* **Weaknesses**
    - I think the main issue is that the author should clarify why the three criteria for biological plausibility are important, for example, through ablation studies or theoretical proofs. This would enhance the scientific value of the paper.
    - Although biological plausible local loss and asymmetric weights are used, gradient descent is still employed for training in this paper. Could this be the main reason why DLL outperforms previous work? An important criterion of brain-inspired learning rules is to abandon GD (such as STDP), because the brain does not directly compute gradients. 



## Other Comments Or Suggestions*
> If you have any other comments or suggestions (e.g., a list of typos), please write them here.

No.


## Questions For Authors*
> If you have any important questions for the authors, please carefully formulate them here. Please reserve your questions for cases where the response would likely change your evaluation of the paper, clarify a point in the paper that you found confusing, or address a critical limitation you identified. Please number your questions so authors can easily refer to them in the response, and explain how possible responses would change your evaluation of the paper.

Please see weaknesses.



## Overall Recommendation*

- [] 5: Strong accept
- [] 4: Accept
- [x] 3: Weak accept (i.e., leaning towards accept, but could also be rejected)
- [] 2: Weak reject (i.e., leaning towards reject, but could also be accepted)
- [] 1: Reject