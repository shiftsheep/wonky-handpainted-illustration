---
name: wonky-handpainted-illustration
description: Generate or edit cohesive characters, achievement badges, app icons, and illustrations in a cute-but-not-childish wonky hand-painted style. Use when the user wants deliberately imperfect flat shapes, restrained exaggeration, dry gouache or crayon texture, or a reusable visual family across app assets.
---

# 粗拙手绘插画

生成一套“略粗糙、略笨拙、可爱但不幼稚”的平面手绘视觉。风格服务于主体识别，不得把任何示例角色、物种或品种固化为默认形象。

## 内置风格锚点

生成时将 [style-reference.jpg](assets/style-reference.jpg) 作为风格参考，而不是固定猫角色模板。只借鉴其中的粗拙轮廓、扁平色块、手绘肌理、克制夸张和系列资产一致性；不得复制示例中的猫、配色或构图。始终把用户提供的身份参考与该风格参考分开标注和使用。

## 开始前

先记录以下变量。不得在变量未入表时直接生成；缺失项可从用户上下文或参考图合理推断并明确标注假设，不适用项写“无”：

- `模式`：角色形象 / 成就徽章 / APP Icon / 单幅或场景插画
- `主体`：角色、物件或概念
- `物种/类别`：动物物种或非动物对象类别
- `品种/子类`：影响外形的细分类；不适用时也需明确为“无”
- `身份特征`：体态、脸型、花纹、配色、服饰、道具、神态等不可丢失的特征
- `用途与交付`：画布比例、真实目标像素尺寸、导出格式、背景实色/透明需求、平台规则与是否需要系列化

若用户给了参考图，先区分“身份参考”与“风格参考”。只提取用户要求的内容，不把参考图中的背景、构图或无关细节带入成品。

## 工作流

1. 阅读 [design-language.md](references/design-language.md)，建立共同风格约束。
2. 只阅读当前模式对应的 [asset-modes.md](references/asset-modes.md) 小节。
3. 从 [prompt-recipes.md](references/prompt-recipes.md) 选择模板，填满变量后再调用图像生成或编辑工具。编辑已有图像时必须包含目标图；有身份参考图时也必须包含。
4. 生成后按 [qa-checklist.md](references/qa-checklist.md) 做视觉检查。
5. 若需迭代，每轮只改变一个视觉变量，锁定其余已认可特征。

## 不可妥协的约束

- 造型来自略歪、略钝、略不对称的轮廓和克制的比例夸张，不靠巨眼、腮红或婴儿化比例卖萌。
- 使用有限的平面色块与干水粉、蜡笔或粗铅笔质感；纹理应属于笔触和覆盖关系，不是覆盖全图的统一噪点滤镜。
- 保留轻微越界、漏白、覆盖不均与手绘错位，但主体剪影必须清晰。
- 用户明确的物种、品种与身份特征优先级高于风格。不得用“粗拙”作为画错结构、花纹位置或关键识别特征的理由。
- 先做大形与层级，再补最少的识别细节。避免毛发级刻画、写实光影、精密矢量边缘和装饰堆砌。
- 多资产输出必须共享造型逻辑、色彩关系、纹理密度与夸张尺度，但允许构图因用途而异。
