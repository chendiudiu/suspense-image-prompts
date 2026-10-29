# 悬疑图片提示词优化

一个用于优化悬疑图片生成提示词的 Codex 技能，支持单张画面、故事配图和连续分镜。

它将抽象的恐惧转成可见线索，调整构图与景别，检查人物、道具和场景连续性，并安排线索与反转的信息揭示。默认保留原故事、分镜数量和顺序；涉及剧情的修改单独列为建议。

## 使用

安装技能后，在对话中调用：

```text
使用 $suspense-image-prompts 优化以下悬疑图片提示词，保留原故事和分镜顺序。
```

随后附上原提示词、分镜文本或文档，以及需要保留的画幅、风格和角色设定。

## 文件

- `suspense-image-prompts/SKILL.md`：技能入口与优化规则。
- `suspense-image-prompts/agents/openai.yaml`：技能显示名称与默认调用提示。
- `suspense-image-prompts/references/examples.md`：城市走廊、日间办公室与巨骨反转等改写示例。
- `suspense-image-prompts.zip`：完整技能包。

技能默认只编写和优化提示词，不自动调用图片生成工具。结构校验已通过；提示词对具体模型的出图效果仍需实际验证。
