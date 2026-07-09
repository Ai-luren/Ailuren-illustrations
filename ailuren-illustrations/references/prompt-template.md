# 生图提示词模板

每张图单独生成。根据正文内容替换变量，不要把多张图拼在一起。

```text
Generate one standalone 16:9 horizontal Chinese article illustration.

Visual DNA:
Pure white background. Minimalist black hand-drawn line art. Slightly wobbly pen lines. Lots of empty white space. Sparse red/orange/blue handwritten Chinese annotations. Clean slightly-absurd product-sketch feeling. No gradients, no paper texture, no complex background, no commercial vector style, no PPT infographic look, no cute mascot poster, no children's illustration, no realistic UI.

Recurring IP character required:
Ai路人, a simple white rounded humanoid passerby character with a round head, smooth connected body, rounded arms and legs, no clothes, no mouth, no nose, and two black vertical oval eyes. Ai路人 must perform the core conceptual action, not decorate the scene. On the white background, keep the white body visible with a clear black outline and an optional local black backdrop / portal / shadow patch behind the character. Make Ai路人 quiet, curious, serious, deadpan, and slightly strange, not cute, not a robot, not an astronaut, not a toy.

Theme:
{正文配图主题}

Structure type:
{结构类型：Workflow / 系统局部 / 前后对比 / 角色状态 / 概念隐喻 / 方法分层 / 地图路线 / 小漫画分镜}

Core idea:
{这张图要表达的核心意思}

Composition:
{具体画面：Ai路人在哪里、正在做什么、主要物件是什么、信息如何流动}

Suggested elements:
{元素1} / {元素2} / {元素3} / {元素4}

Chinese handwritten labels:
{标注词1} / {标注词2} / {标注词3} / {标注词4} / {可选标注词5}

Color use:
Black for continuous hand-drawn line art, labels, structure, Ai路人的 oval eyes / outline, and optional local black backdrop. White for Ai路人的 body and background. Orange for main flow/path/arrows. Red only for key warnings/problems/results. Blue only for secondary notes or feedback/system state. No gray anywhere. No dashed lines or dotted lines.

Constraints:
One image explains only one core structure. Keep the main subject around 40%-60% of the canvas. Preserve at least 35% blank white space. Use at most 5-8 short handwritten Chinese labels. Do not write a title in the top-left corner. Do not write the structure type on the image. Do not make it a formal diagram, course slide, or dense explainer. Do not make Ai路人 black, over-detailed, cute, toy-like, robotic, or dressed. Do not use gray lines, gray fills, gray shadows, dashed lines, dotted lines, engineering guide lines, or sketch construction lines. Do not copy prior examples or reuse known case compositions unless explicitly requested; invent a fresh visual metaphor for this specific article. It should be clear but not instructional, interesting but not childish, strange but clean.
```

## 图像编辑提示

去掉左上角标题：

```text
Edit the provided image. Remove only the handwritten title "{要删除的文字}" and its underline from the top-left corner. Fill that area with the same clean white background, matching the surrounding blank paper. Preserve everything else exactly: characters, labels, paths, line style, composition, aspect ratio, and image quality. Do not add any new text or objects.
```

增强参与感：

```text
Regenerate this illustration with the same core meaning and simple layout, but make Ai路人 more central to the conceptual action. Ai路人 should be doing the work that explains the idea, not standing beside the diagram. Keep the character white, rounded, mouthless, with black oval eyes and a visible outline on the white background. Keep it clean, sparse, hand-drawn, and not cute.
```
