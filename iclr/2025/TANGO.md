### TANGO: CO-SPEECH GESTURE VIDEO REENACTMENT WITH HIERARCHICAL AUDIO MOTION EMBEDDING AND DIFFUSION INTERPOLATION
1. 提出了一种根据audio生成video的pipeline
2. 需要给出reference video, 然后通过一个graph和CLIP寻找一段audio最优的匹配frame
3. 通过diffusion在frame之间插帧生成