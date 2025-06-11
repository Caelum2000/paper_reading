### TRUST OR ESCALATE: LLM JUDGES WITH PROVABLE GUARANTEES FOR HUMAN AGREEMENT
1. LLM judge的研究工作
2. 对每一个LLM judge给出一个置信概率，即是否符合人类perference的概率
3. 级联的进行eval，先用一个弱LLM进行eval，看是否符合概率threshold，若不符合，则用更强的，见Fig.1