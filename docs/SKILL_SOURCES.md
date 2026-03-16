# 已收录来源

本项目的 SKILL 内容综合参考了以下开源项目的实践经验和设计思路。

---

## 直接参考来源

| 来源 | 贡献内容 | 吸收到哪个 SKILL | 链接 |
|------|---------|-----------------|------|
| xstongxue/best-skills | 论文大纲审核、章节仿写、润色去AI味 | 03-大纲生成、04-章节写作、08-AI痕迹消除 | [GitHub](https://github.com/xstongxue/best-skills) |
| wanddream/skill-thesis-writer | 中文学位论文全流程审查、AI痕迹消除 | 05-全文审查、08-AI痕迹消除 | [GitHub](https://github.com/wanddream/skill-thesis-writer) |
| huangkiki/dailypaper-skills | 文献筛选与阅读辅助 | 02-文献分析 | [GitHub](https://github.com/huangkiki/dailypaper-skills) |
| junkzhu/Chinese-Dissertation-Writing-Skill | 风格迁移、错题本机制、一致性检查 | 00-风格学习、06-一致性检查 | [GitHub](https://github.com/junkzhu/Chinese-Dissertation-Writing-Skill) |
| Stars-OC/thesis-creator | 全流程工作流设计、AIGC检测、降重优化 | 07-降重改写、整体流程设计 | [GitHub](https://github.com/Stars-OC/thesis-creator) |
| LeonChaoX/qinyan-academic-skills | 学术Skill分类体系、文献检索Skill | 项目结构参考 | [GitHub](https://github.com/LeonChaoX/qinyan-academic-skills) |
| RETHINKAIZ/thinking-order-skills | 改写降重、文风润色、选题策划 | 07-降重改写、01-选题调研 | [GitHub](https://github.com/RETHINKAIZ/thinking-order-skills) |

---

## 设计理念来源

- **风格DNA提取**：思路源自 junkzhu 的 style_extractor，适配为网页版单次对话的即时提取方案
- **错题本机制**：思路源自 junkzhu 的 error_log，在网页版中转化为 SKILL 内预置的常见错误规则库
- **双层降重策略**：受 Stars-OC 的 synonym_replace.py + LLM 改写启发，在纯 prompt 形态中转化为5级改写策略体系
- **8种AI痕迹特征**：综合了 wanddream、xstongxue 的去AI味规则和实际 AIGC 检测工具的判定标准

---

## 贡献新来源

如果你发现了其他优秀的论文写作相关 Skill/Prompt 项目，欢迎通过以下方式提交：

1. 提 Issue，附上项目链接和你认为值得参考的内容
2. 提 PR，直接更新本文件并说明吸收了什么内容

收录标准：
- 必须是开源项目
- 内容与中文学位论文写作相关
- 有可借鉴的规则、策略或设计思路
