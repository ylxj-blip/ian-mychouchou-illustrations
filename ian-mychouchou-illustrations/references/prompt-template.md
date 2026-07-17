# 生图提示词模板

每张图单独生成。根据正文内容替换变量，不要把多张图拼在一起。

```text
Generate one standalone 16:9 horizontal Chinese article illustration.

Visual DNA:
Pure white background. Minimalist black hand-drawn line art. Slightly wobbly pen lines. Lots of empty white space. Sparse red/orange/blue handwritten Chinese annotations. Clean absurd product-sketch feeling. Simplified cartoon drawing, not realistic rendering. No gradients, no shadows, no paper texture, no complex background, no commercial vector style, no PPT infographic look, no cute mascot poster, no children's illustration, no realistic UI, no realistic fur rendering.

Recurring IP character required:
mychouchou, a sturdy medium-long-haired ragdoll cat mascot with a round face, large round blue eyes, a cream-gray and white bicolor face mask, pink nose and mouth, high pointed ears, fluffy chest ruff, soft long-haired torso, medium-length legs, and a fluffy tail. The body should feel balanced,健硕, and slightly majestic like a tiny lion, but not fat, not short-legged, not lanky, and not over-fluffed. mychouchou must perform the core conceptual action, not decorate the scene. Make mychouchou gentle, innocent, quietly adorable, and clearly cartoon-hand-drawn rather than realistic pet-like.

Reference-face policy:
If a confirmed mychouchou reference image is available in the conversation or provided by the user, treat that image as the highest-priority identity anchor. Match its face proportions, eye size, facial mask pattern, torso fluff level, leg proportion, tail fluff, and overall cartoon simplification before matching any new pose details.

One-word recognition point:
狮偶

Identity anchors that must not drift:
- match the confirmed mychouchou reference face first
- preserve the stable cream-gray bicolor ragdoll face mask and white central face area
- preserve the big round blue eyes and soft pink nose/mouth
- preserve the long-haired ragdoll torso instead of a short-haired body
- preserve medium-length legs: not stubby, not tall
- preserve mild lion-like dignity without becoming wild or over-fluffy
- preserve the same cartoon simplification level across images
- keep the same overall species read and silhouette
- first see it working, then see it cute

Theme:
{正文配图主题}

Structure type:
{先判断后的单一主结构：层级 / 交集 / 二维分类 / 并列分组 / 流程路径 / 系统局部 / 前后对比 / 角色状态 / 概念隐喻 / 方法分层 / 地图路线 / 小漫画分镜}

Core idea:
{这张图要表达的核心意思}

Composition:
{具体画面：mychouchou 在哪里、正在做什么、主要物件是什么、信息如何流动；只保留一个主结构，不混搭}

Suggested elements:
{元素1} / {元素2} / {元素3} / {元素4}

Chinese handwritten labels:
{标注词1} / {标注词2} / {标注词3} / {标注词4} / {可选标注词5}

Color use:
Black for main line art and structure. Use the confirmed mychouchou body colors from the reference image. Orange for main flow/path/arrows. Red only for key warnings/problems/results. Blue only for secondary notes or feedback/system state.

Constraints:
One image explains only one core structure. Keep the main subject around 40%-60% of the canvas. Preserve at least 35% blank white space. Use at most 3-6 short handwritten Chinese labels by default, only expand to 8 if truly necessary. Do not write a title in the top-left corner. Do not write the structure type on the image. Do not generate long Chinese sentences or paragraph text inside the image. Do not make it a formal diagram, course slide, or dense explainer. Do not copy prior examples or reuse known case compositions unless explicitly requested; invent a fresh visual metaphor for this specific article. It should be clear but not instructional, interesting but not childish, strange but clean.

Hard constraints for mychouchou:
- do not drift away from the confirmed mychouchou reference face
- do not invent new facial markings or body patterns
- do not make the torso read as a short-haired cat
- do not make the body chubby-fat, stubby, or dumpling-like
- do not make the legs too short or too long
- do not turn the fluff into an explosive furball
- do not make mychouchou look like a pet sticker, emoji animal, plush toy, or baby mascot
- do not make it passive; it must visibly operate, carry, pull, push, guide, inspect, or block something
- do not render detailed fur, realistic shading, or realistic anatomy
- if the character is removed and the image still fully works, the prompt has failed

Text-generation policy:
- prefer image-without-title
- prefer short labels over sentences
- if the task is closer to a formal infographic, generate the visual skeleton only: cat, icons, groups, arrows, containers, and blank label areas
- let external layout tools add precise Chinese typography later

Generation priority order:
1. match the confirmed mychouchou reference face
2. preserve the working-cat feeling
3. preserve the hand-drawn cartoon style
4. preserve the scene structure
5. add labels only if needed
```

## 图像编辑提示

去掉左上角标题：

```text
Edit the provided image. Remove only the handwritten title "{要删除的文字}" and its underline from the top-left corner. Fill that area with the same clean white background, matching the surrounding blank paper. Preserve everything else exactly: characters, labels, paths, line style, composition, aspect ratio, and image quality. Do not add any new text or objects.
```

增强怪诞感：

```text
Regenerate this illustration with the same core meaning and simple layout, but make mychouchou more central to the conceptual action. mychouchou should be doing the strange work that explains the idea, not standing beside the diagram. Keep it clean, sparse, hand-drawn, and not pet-like.
```
