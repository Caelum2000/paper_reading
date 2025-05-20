### INFERENCE SCALING FOR LONG-CONTEXT RETRIEVAL AUGMENTED GENERATION
1. 提出了两种通过增加计算量来提升性能的RAG方法：DRAG和IterDRAG。DRAG具体方法是in-context learning来对LLM RAG的内容进行示范。IterDRAG，是将问题分解为子问题然后call DRAG
2. 研究了计算量增加和RAG效果之间的关系，满足类似scaling law的关系