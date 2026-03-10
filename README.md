# 🎓 thesis-skill-hub

**硕士论文审查与写作 SKILL 聚合项目**

持续收录 GitHub 上最优质的论文写作 skill，归纳为一份可直接使用的 `SKILL.md`。

适用平台：Claude / ChatGPT / Gemini 网页版（无需 CLI、无需编程）

---

## 这是什么？

写硕士论文时，GitHub 上有很多优秀的 AI 写作辅助 skill（提示词工程文件），但它们散落在不同仓库里，每个人都要自己找、自己对比、自己合并。

本项目做的事情很简单：**帮你把这些 skill 收集起来，去重、合并、优化，输出一个可以直接复制粘贴使用的 `SKILL.md`。**

## 30秒上手

1. 打开 [`SKILL.md`](./SKILL.md)，全选复制
2. 打开 [claude.ai](https://claude.ai) 或 [chatgpt.com](https://chatgpt.com)，新建对话
3. 粘贴以下内容：

```
请你完整阅读以下工作指令，阅读完毕后只需回复「已就绪，请提供论文内容」：

【粘贴 SKILL.md 全文】
```

4. 等 AI 回复"已就绪"后，上传你的论文 PDF
5. 发送：`请按照SKILL中的审查标准进行完整审查`

详细操作见 [`docs/使用说明书.md`](./docs/使用说明书.md)

## 仓库结构

```
thesis-skill-hub/
├── SKILL.md                          # 核心文件：直接复制给AI使用
├── README.md                         # 项目说明（你正在看的）
├── LICENSE                           # MIT许可证
├── docs/
│   ├── 使用说明书.md                  # 详细使用说明（给人看，不给AI）
│   ├── SKILL_SOURCES.md              # 已收录的skill来源清单
│   ├── CHANGELOG.md                  # 更新日志
│   └── CONTRIBUTING.md               # 贡献指南
└── .github/
    ├── ISSUE_TEMPLATE/
    │   ├── recommend-skill.md        # Issue模板：推荐新skill
    │   └── report-problem.md         # Issue模板：报告问题
    └── workflows/
        └── lint.yml                  # GitHub Action：自动检查Markdown格式
```

## 已收录来源

| 来源 | 贡献内容 | 链接 |
|------|---------|------|
| xstongxue/best-skills | 论文大纲审核、章节仿写、润色去AI味 | [GitHub](https://github.com/xstongxue/best-skills) |
| wanddream/skill-thesis-writer | 中文学位论文全流程审查、AI痕迹消除 | [GitHub](https://github.com/wanddream/skill-thesis-writer) |
| huangkiki/dailypaper-skills | 文献筛选与阅读辅助 | [GitHub](https://github.com/huangkiki/dailypaper-skills) |

完整清单见 [`docs/SKILL_SOURCES.md`](./docs/SKILL_SOURCES.md)

## 如何贡献

发现了好用的论文写作 skill？欢迎通过以下方式参与：

- 🐛 **提 Issue：** 使用 [推荐新skill](../../issues/new?template=recommend-skill.md) 模板
- 💬 **参与讨论：** 在 [Discussions](../../discussions) 中交流
- 🔧 **提交 PR：** 详见 [`docs/CONTRIBUTING.md`](./docs/CONTRIBUTING.md)

## 维护节奏

- 每周检查一次 PR 和 Issues
- 审核通过的内容合并进 `SKILL.md`
- 所有变更记录在 [`docs/CHANGELOG.md`](./docs/CHANGELOG.md)
- `main` 分支受保护，所有修改必须通过 PR + Review

## 适用范围

- ✅ 理工科硕士学位论文（6章结构为主，5章/7章可类比）
- ✅ Claude / ChatGPT / Gemini 网页版
- ✅ 中文论文（GB/T 7714-2015 参考文献标准）
- ⚠️ 文科/社科论文需根据学科特点调整部分规则
- ⚠️ 博士论文可参考，但深度和广度要求更高

## 许可证

[MIT License](./LICENSE) — 随便用，注明出处就行。

---

> 💡 本项目由一个即将毕业的电气工程硕士发起，在自己写论文的过程中整理而成。如果对你有帮助，给个 ⭐ Star 就是最大的支持。
