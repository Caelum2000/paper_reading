# Title SpikeVFuse: Enhancing Infrared and Visible Image Fusion with Spiking Neural Networks

# Review Form (Transcribed from Figures)

## A. Suitability of Topic

### A.1. Is the topic appropriate for publication in these transactions? — NEW
- [ ] Excellent Match  
- [x] Adequate Match  
- [ ] Poor Match  

---

## B. Content

### 1. Is the paper technically sound?
- [x] Yes  
- [ ] No  

### 2. How would you rate the technical novelty of the paper?
- [ ] Very Novel  
- [x] Novel Enough for Publication  
- [ ] Not Novel  

**Explain:**  
> (Text box)
This work proposes a spiking-neural-network–based image fusion pipeline and demonstrates promising performance compared with existing baselines. The authors further claim that the proposed framework achieves lower energy consumption than conventional approaches. However, the novelty of the work may be somewhat limited, as image fusion has become a relatively mature research topic, especially in comparison with recent advances in large-scale vision generative foundation models such as Stable Diffusion or DALL·E.

### 3. Is the contribution significant?
- [ ] Significant  
- [ ] Moderately Significant  
- [x] Incremental  
- [ ] Not Significant  

### 4. Is the coverage of the topic sufficiently comprehensive and balanced?
- [ ] Yes  
- [x] Treatment somewhat unbalanced, but not seriously so  
- [ ] Important information is missing or superficially treated  

### 5. Rate the Bibliography
- [x] Satisfactory  
- [ ] Unsatisfactory  

---

## C. Presentation

### 1. How would you rate the overall organization of the paper?
- [x] Satisfactory  
- [ ] Could be improved  
- [ ] Poor  

### 2. Are the title and abstract satisfactory?
- [x] Yes  
- [ ] No  

### 3. Is the length of the paper appropriate?  
- [x] Yes  
- [ ] No (Explain):  
> (Text box)

### 4. Are symbols, terms, and concepts adequately defined?
- [x] Yes  
- [ ] Not always  
- [ ] No  

### 5. How do you rate the English usage?
- [x] Satisfactory  
- [ ] Needs improvement  
- [ ] Poor  

---

## D. Suggested References

If you are suggesting additional references they must be entered below. All suggestions must include full bibliographic information plus a DOI.

If not suggesting references, type **N/A**.

> (Text box)

N/A

## Recommendation

- [ ] A — Publish Unaltered  
- [x] AQ — Publish With Minor Required Changes  
- [ ] RQ — Review Again After Major Changes  
- [ ] R — Reject  

---

## Confidential Comments to the Associate Editor
> (Text box)

This manuscript proposes a spiking neural network–based image fusion framework and introduces several technical innovations, including the SBGC architecture. The experimental results indicate that the method achieves state-of-the-art performance compared with existing baselines, while maintaining exceptionally low parameter count and energy consumption. Although image fusion itself is no longer a highly active or high-impact topic (as noted in the novelty justification), the paper provides a meaningful incremental advancement within this area. Overall, the work has merit and could be considered for publication after appropriate revisions.

## Comments to Author  
Please state why you rated the paper as you did. If revisions are required, give specific guidance, distinguishing between optional and mandatory changes.

> (Text box)

--- 

1. One of the manuscript’s central claims is that the proposed spiking model is energy-efficient. In Section V.D, however, the energy consumption is estimated only through theoretical calculations rather than measurements on real hardware. It is recommended that the authors discuss the potential gap between theoretical estimates and actual energy consumption on neuromorphic or conventional hardware, which would make the argument more solid and comprehensive.

2. The proposed image fusion model includes the “SBGC” module described in Section IV.B. This structure resembles the widely used Mixture-of-Experts (MoE) paradigm. It is suggested that the authors discuss the relationship between SBGC and MoE, particularly regarding how the spiking time-step dynamics influence sub-network selection within SBGC. Additionally, providing a more detailed and mathematically grounded description of the SBGC mechanism in Section IV.B would further clarify its design and improve technical rigor.

3. In the experimental section, additional ablation studies would strengthen the paper. In particular, isolating and evaluating the individual contributions of the SDBC and SBGC modules would help clarify their respective roles and quantify their impact on the overall performance.

## Attach Files
(Max of 10 at a time)

N/A