### BACKTRACKING IMPROVES GENERATION SAFETY
1. 提出backtracking方法，就是让LLM能够生成一种特殊token，[RESET]。
2. [RESET]能够撤销之前生成的内容，从而在已经生成unsafe之后检测并撤销。作者发现这样能够enhance safe的程度
3. 修正了loss，见Eq.1。加了额外的一项，鼓励在生成undesirable内容后生成[RESET]撤回。这其实是一种对齐