### Partial Identification of Treatment Effects with Implicit Generative Models
1. 和NCM那篇论文差不多，都是研究不能identifiable的情况下（例如有unobserved cofounder）ATE的bound。
2. 通过minmax优化得到了不能辨识的情况下的ATE的bound
3. 为什么unobserved cofounder会导致不能辨识的问题？因为学到的只能是p(y|t)
4. 这一篇和NCM都是因果辨识的问题，NCM是研究的是基于目前的graph否可以辨识，这篇是不能辨识的情况下给出一个bound