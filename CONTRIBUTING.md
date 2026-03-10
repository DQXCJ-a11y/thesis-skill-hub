# 🤝 贡献指南

感谢你考虑为 thesis-skill-hub 做贡献！

---

## 如何贡献

### 方式一：推荐新的 Skill 来源（最简单）

点击 [推荐新skill](../../issues/new?template=recommend-skill.md)，按模板填写即可。

### 方式二：参与讨论

在 [Discussions](../../discussions) 中交流：
- 分享你发现的好用 skill
- 讨论 SKILL.md 的改进方向
- 反馈使用体验

### 方式三：提交 Pull Request

1. Fork 本仓库
2. 创建新分支：`git checkout -b add/new-skill-source`
3. 修改对应文件
4. 提交 Pull Request

#### PR 应包含

- [ ] 来源链接（必须）
- [ ] 简要说明这个来源的亮点
- [ ] 该内容是否已合并到 SKILL.md
- [ ] 已在 `docs/CHANGELOG.md` 中记录变更

#### 审核标准

- 内容必须是公开的、可合法使用的
- 必须标注原始出处
- 符合现有 SKILL.md 的格式规范
- 不与现有内容大面积重复

---

## 分支与合并规则

| 规则 | 说明 |
|------|------|
| ✅ 只有维护者直接 merge PR | 所有PR都需要 code review |
| ✅ `main` 分支受保护 | 不能直接 push，必须通过 PR |
| ✅ 每次合并记录到 CHANGELOG | 标注来源、修改者、日期 |
| ✅ 每周整理更新一次 | 集中处理积压的 PR 和 Issue |

---

## 维护流程

```
周期性维护（每周一次）：

1️⃣ 检查 PR 和 Issues
2️⃣ 审核新提交的 skill 来源
3️⃣ 用 AI 辅助提取有价值的规则/模板/清单
4️⃣ 合并进 SKILL.md
5️⃣ 更新 docs/SKILL_SOURCES.md（添加新来源）
6️⃣ 更新 docs/CHANGELOG.md（记录变更）
7️⃣ 关闭已处理的 PR 和 Issue
```

---

## CHANGELOG 记录格式

每次更新时按以下格式记录：

```markdown
## [日期]

### Added
- 来自 @贡献者 的 XXX 内容
  来源：https://github.com/xxx/xxx

### Updated
- 完善了 XXX 部分的文档

### Contributors
- @维护者
- @贡献者
```

---

## 不适合的贡献

- ❌ 与论文写作无关的 skill（如代码 review、产品文档等）
- ❌ 纯英文论文的 skill（本项目当前聚焦中文学位论文）
- ❌ 需要付费才能使用的 skill 或工具
- ❌ 包含具体论文内容的提交（涉及学术诚信）
- ❌ 未标注来源的内容

---

## 额外说明

### Issue 模板

本仓库提供了两个 Issue 模板：
- **推荐新skill：** 发现好用的论文 skill 时使用
- **报告问题：** SKILL.md 中有错误或需要改进时使用

### GitHub Discussions

非正式的交流请使用 Discussions，适合：
- 讨论某个 skill 的优劣
- 分享使用心得
- 提出改进想法（还没想清楚的）

### GitHub Actions

仓库配置了自动化检查：
- PR 提交时自动检查 Markdown 格式
- 确保文件结构符合规范

---

感谢每一位贡献者！🎓
