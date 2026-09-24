# x-content-studio-cn

面向中文 X 创作者的 Codex Skill，用于研究、写作、审校、视觉规划与发布后复盘。

它适合 AI、科技、金融、加密货币和经济评论等方向，强调：

- 先核验来源，再写观点；
- 区分事实、推断与个人判断；
- 默认生成一篇完整的中文蓝 V 长帖，而不是机械拆分 Thread；
- 配图承担解释或证据作用，不把生成图伪装成真实截图；
- 保留人工终审，不读取 Cookie，也不自动发布。

## 安装

将本仓库克隆或下载到项目的 `.agents/skills/x-content-studio-cn`：

```text
your-project/
└─ .agents/
   └─ skills/
      └─ x-content-studio-cn/
```

也可以安装到个人 Codex skills 目录，以便在多个项目中使用。

## 使用方式

在 Codex 中直接提出类似请求：

- “生成今天的 X 推文，先扫描热点再选题。”
- “把这条公开帖子改写成有证据边界的引用观点。”
- “写一篇 Codex 教程，并规划三张配图。”
- “根据真实发布数据复盘这篇推文。”

Skill 会根据任务读取对应参考文件，并把账号权限与发布动作保留给用户。

## 目录

```text
x-content-studio-cn/
├─ SKILL.md
├─ agents/
│  └─ openai.yaml
└─ references/
   ├─ chinese-voice.md
   ├─ post-formats.md
   ├─ research-and-evidence.md
   ├─ review-and-metrics.md
   └─ visual-system.md
```

## 安全边界

本 Skill 不会发布、回复、点赞、转发、关注或发送私信，也不会读取账号 Cookie。公开发布需要独立工具和用户单独授权。

## License

[MIT](LICENSE)
