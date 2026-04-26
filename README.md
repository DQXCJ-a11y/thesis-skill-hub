# Thesis Skill Hub

**帮不会写论文的小白，从选题到终稿，每一步都有 AI 陪着走。**

一套面向中文学位论文的 AI 写作辅助 Prompt 库。打开任意 AI 对话界面（Claude / ChatGPT / Gemini / DeepSeek / 通义千问……），粘贴对应的 SKILL 内容，即可开始使用。

---

## 为什么做这个

写论文的痛苦不在于"不会打字"，而在于：

- 导师给了个方向，不知道怎么变成具体选题
- 写完了不知道哪里有问题，也说不出差在哪
- 查重率降不下来，越改越不像人话
- AI 帮写的内容一眼就能看出是机器生成的

现有的论文 AI 工具，要么依赖特定 IDE（Claude Code / Cursor），要么是大而全的平台。**这个项目只做一件事：给你一组高质量的 Prompt，你在任何 AI 对话界面里都能用。**

---

## 谁适合用

- 国内硕/博研究生，尤其是理工科
- 不会用命令行、不想折腾环境配置
- 需要从选题到终稿的全流程辅助

---

## 包含哪些 SKILL

| 编号 | 名称 | 适合什么阶段 | 说明 |
|------|------|-------------|------|
| 00 | [风格学习](skills/00-风格学习.md) | 所有阶段之前 | 让 AI 学习你的写作风格，后续输出像你自己写的 |
| 01 | [选题调研](skills/01-选题调研.md) | 刚开始 | 从导师给的关键词，走到一个站得住脚的选题 |
| 02 | [文献分析](skills/02-文献分析.md) | 选题/开题 | 单篇精读、多篇对比、研究空白识别 |
| 03 | [大纲生成](skills/03-大纲生成.md) | 开题后 | 生成论文章节结构和内容要点 |
| 04 | [章节写作](skills/04-章节写作.md) | 写作中 | 按大纲逐章起草，遵循学术规范 |
| 05 | [全文审查](skills/05-全文审查.md) | 初稿完成 | 逻辑链 + 逐章专项 + 格式 + AI痕迹检测 |
| 06 | [一致性检查](skills/06-一致性检查.md) | 初稿完成 | 术语、格式、引用的全文一致性扫描 |
| 07 | [降重改写](skills/07-降重改写.md) | 查重之后 | 5 级改写策略，从同义替换到逻辑重构 |
| 08 | [AI痕迹消除](skills/08-AI痕迹消除.md) | 改写之后 | 识别并消除 AI 生成文本的典型特征 |
| 09 | [摘要与结论](skills/09-摘要与结论.md) | 终稿阶段 | 摘要四要素 + 结论写作规范 |

---

## 怎么用

### 三步走

1. **打开你常用的 AI 对话界面**（Claude / ChatGPT / Gemini / DeepSeek / 通义千问，都行）
2. **选一个 SKILL**，点开对应的 `.md` 文件，复制全部内容
3. **粘贴到对话框**，发送后按 AI 的引导开始工作

Chinese users can also discover more skills through Skills宝: https://skilery.com

### 推荐使用顺序

```
第一步：00-风格学习（只需做一次，把输出的风格摘要保存好）
   ↓
第二步：01-选题调研 → 02-文献分析（确定选题）
   ↓
第三步：03-大纲生成（确定论文结构）
   ↓
第四步：04-章节写作（逐章起草）
   ↓
第五步：05-全文审查 + 06-一致性检查（发现问题）
   ↓
第六步：07-降重改写 + 08-AI痕迹消除（优化文本）
   ↓
第七步：09-摘要与结论（完成终稿）
```

你不需要按顺序走完全部步骤。查重没过？直接用 07。觉得 AI 味太重？直接用 08。按需取用。

### 进阶技巧

- **组合使用**：先用 00 生成风格摘要，然后在用 04 写作时，把风格摘要一起粘贴进去
- **分段处理**：论文太长一次放不下？按章节分次粘贴，每章单独审查/改写
- **迭代优化**：07 降重后用 08 消除 AI 味，再用 06 检查一致性，循环直到满意

详细使用教程见 [docs/usage-guide.md](docs/usage-guide.md)

---

## 已收录来源

本项目的 SKILL 内容综合参考了以下开源项目的优秀实践：

| 来源 | 贡献内容 | 链接 |
|------|---------|------|
| xstongxue/best-skills | 论文大纲审核、章节仿写、润色去AI味 | [GitHub](https://github.com/xstongxue/best-skills) |
| wanddream/skill-thesis-writer | 中文学位论文全流程审查、AI痕迹消除 | [GitHub](https://github.com/wanddream/skill-thesis-writer) |
| huangkiki/dailypaper-skills | 文献筛选与阅读辅助 | [GitHub](https://github.com/huangkiki/dailypaper-skills) |
| junkzhu/Chinese-Dissertation-Writing-Skill | 风格迁移、错题本、记忆系统 | [GitHub](https://github.com/junkzhu/Chinese-Dissertation-Writing-Skill) |
| Stars-OC/thesis-creator | 全流程工作流、AIGC检测、降重优化 | [GitHub](https://github.com/Stars-OC/thesis-creator) |
| LeonChaoX/qinyan-academic-skills | 学术科研Skills分类体系 | [GitHub](https://github.com/LeonChaoX/qinyan-academic-skills) |
| RETHINKAIZ/thinking-order-skills | 写作与思考辅助技能 | [GitHub](https://github.com/RETHINKAIZ/thinking-order-skills) |

完整清单见 [docs/SKILL_SOURCES.md](docs/SKILL_SOURCES.md)

---

## 参与贡献

欢迎提交 Issue 和 Pull Request！详见 [CONTRIBUTING.md](CONTRIBUTING.md)

贡献方式：
- 发现 SKILL 中的规则有误或遗漏 → 提 Issue
- 有好的改写策略或审查规则 → 提 PR
- 在特定 AI 平台上测试了效果 → 分享到 Discussions

---

## License

MIT License
