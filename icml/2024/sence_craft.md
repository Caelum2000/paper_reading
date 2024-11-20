## SceneCraft: An LLM Agent for Synthesizing 3D Scenes as Blender Code
1. 利用llm写blender的脚本
2. 分inner-loop和outer-loop
3. inner loop就是不断生成代码，然后利用另一个LVM评价blender渲染的场景，不断refine
4. outer loop好像就是更新一个library