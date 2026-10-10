# Punk IP Video Cover

**Punk 出品｜上传人物照片，按主题与标题制作人物 IP 视频封面。**

这是一个 Agent Skill：从本期照片提取四个代表色并搭配，抠出真人主体，再按主题与标题自由构图，结合风格库处理字体、材质与装饰，输出可直接使用的视频封面。

`Punk` 是作者印记与示例，不代表只能做 Punk。任何人都可以上传自己的照片，做自己的人物封面。

## 适合做什么

- 小红书 / Shorts / 横版视频封面
- 同一人物、同一主题出多个风格或排版版本
- 3:4、16:9、4:3、9:16 等比例（未指定时默认 3:4）

## 完整流程

```text
上传人物照片
    ↓
提取四个代表色并分配用途
    ↓
抠出真人主体（可改动作与表情）
    ↓
按主题与标题自由构图
    ↓
套用所选风格的字形 / 材质 / 装饰
    ↓
按比例生成封面并检查交付
```

## 安装

克隆到助手的 skills 目录，例如 Codex：

```bash
git clone https://github.com/adrianpunk/punk-ip-video-cover.git ~/.codex/skills/punk-ip-video-cover
```

确认目录内有 `SKILL.md`，重启或刷新助手后即可调用。

## 仓库结构

```text
SKILL.md          # 主流程与规则
agents/           # 助手元数据
styles/           # 风格库（各含 STYLE.md / PROMPT.md）
```

当前风格库约 25 个方向，覆盖撕纸拼贴、Y2K、手写记录、海报、对话框等。实际风格以 `styles/*/STYLE.md` 为准。

## 使用注意

- 有标题时尽量逐字保留；只有主题时可提炼封面标题，不编造成果或数据。
- 默认允许按主题改动作与表情，身份仍须可辨认。
- 不把采集参考图、研究截图或他人封面送进生成链路。
- 本仓库只含文字规则与风格文档，不含研究画廊或成品图样本。

## 相关

- 文章插图技能：[punk-ip-illustrations](https://github.com/adrianpunk/punk-ip-illustrations)
- 作者：[@AdrianPunk115](https://x.com/AdrianPunk115)
