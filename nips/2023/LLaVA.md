## Title: Visual Instruction Tuning
1. 提出用图片进行instruction。具体就是让模型回答图片相关的问题
2. 用CLIP提取图片特征，并用一个W投影到 LLM 的 token embedding
3. 两阶段训练，第一阶段仅仅训练W。第二阶段全训练