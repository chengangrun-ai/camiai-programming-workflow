# camiAI 编程全流程

一个面向 Codex 的可复用 Skill，帮助按固定顺序开发多个产品，并在每个产品中按需跳过产品设计或技术设计。

## 默认流程

1. 环境搭建：检查 Git、项目说明和 `AGENTS.md`。
2. 产品设计：讨论产品方案、MVP，并按需制作模拟数据 Demo。可跳过。
3. 技术设计：讨论并记录认可的技术方案。可跳过。
4. 产品实现：写代码、更新测试、运行验证，并为每个完成的改动建立 Git commit。
5. 人工验证：由用户实际体验，提供反馈后继续修正。

用户可以按产品明确跳过第 2、3 步；默认按顺序执行。提示词模板见 [`references/prompts.md`](references/prompts.md)。

## 安装

把整个 Skill 文件夹复制到 Codex 的 skills 目录：

- Windows 默认路径：`%USERPROFILE%\.codex\skills\camiai-programming-workflow`
- 如果设置了 `CODEX_HOME`，使用 `%CODEX_HOME%\skills\camiai-programming-workflow`

之后可以输入 `$camiai-programming-workflow` 显式调用；产品开发请求也可以触发自动调用。

## 文件结构

```text
camiai-programming-workflow/
├── SKILL.md
├── README.md
├── LICENSE
├── agents/
│   └── openai.yaml
└── references/
    └── prompts.md
```

## 许可

本项目采用 MIT License，详见 [`LICENSE`](LICENSE)。

