# 司马迁·把事件写成有证据的历史

把事件写成有证据的历史：有资料依据、有使用边界、可复核的中文 Agent Skill。

**把熟悉的思想，变成下一次任务可用的方法。**

适合：整理机构历史、人物故事或长期变化叙事。

交付：明确叙事问题、时期和读者 → 建立事件时间线与来源账本 → 把人物选择放回资源、制度和偶然条件 → 核不同来源的共同出处 → 区分可证事件、因果假设与作者评价 → 交付正文及证据注。

**一分钟看懂**：十年公司史草稿把每次成功都归于创始人远见。

本 Skill 会这样处理：补团队、市场与失败事件，评价旁列证据；不虚构动机或把事后结果写成早有预见。

[用途与同类差异](references/positioning.md)。人物知名度提供发现入口，实际价值来自工作流与可复核产物；不保证星标增长。

## 安装与使用
公开仓库直接提供 Skill，不依赖 GitHub Release。
```sh
npx skills add constantin2088/sima-qian-history-skill
```
也可将仓库内容复制到支持该格式的客户端 Skill 目录，保留以 `sima-qian-history-skill` 命名的文件夹和根目录 SKILL.md。客户端支持范围以其文档为准。安装后提出具体任务，由客户端按描述加载。

**试用任务**：十年公司史草稿把每次成功都归于创始人远见。

## 内容
- [执行说明](SKILL.md)
- [资料卡](references/sources.md)、[工作表](references/frameworks.md)、[边界](references/boundaries.md)
- [三个示例](examples/demo.md)、[十个行为评测场景](evals/test-cases.md)

## 验证与贡献
```sh
python scripts/check_skill.py . --release
python -m unittest discover -s tests -v
python scripts/check_links.py
```
`--release` 是完整性检查参数，不创建 GitHub Release。CI 在每次提交运行上述检查。独立客户端模型行为评测尚未执行；用例、结构检查与实际模型能力分开报告。
修改时提供来源和定位，区分原文与转译；运行检查后直接提交到仓库。不要创建发布附件作为必需安装步骤。系列标识、链接和推荐由总仓库 catalog/skills.json 同步，避免手工修改受管理区块。

## 许可
项目原创内容使用 [MIT](LICENSE)。链接所指第三方作品保留原权利，本仓库不重新许可它们。
