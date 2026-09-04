# 交接档（handoff.md）

> 任何 Agent、任何电脑接手前**必读**；收工时**必更新**。本档只放交接必需的精简资讯，详细脉络放 Obsidian（若有 L3）。

## ⏯️ 目前做到哪

<!-- 最后完成的动作，1-3 句 -->
补完 `README.md`（人类友好导览档），本专案作为「技能测试骨架」现在四个档案齐备：README / AGENTS / handoff / 专案工作流程。任何接手者从 README 即可快速理解本专案来历与用法。

## 🚦 目前状态

<!-- 可运行吗？哪些做一半？ -->
- L1 / L2 / L3：✅ 全部就绪
- `project-init` / `startup` / `shutdown` 三个核心技能在当前环境验证通过
- 路线图阶段一～六全部勾选完成
- 本专案本身不承载业务，作为测试骨架长期保留

## ➡️ 下一步

<!-- 具体可执行 -->
1. （可选）在其他机器（如装了 Obsidian MCP / 装了 `gh` 但未登入的环境）跑一次 startup，验证跨电脑交接
2. （可选）给 README 补一两个截图 / 图示，让导览更友善
3. 收工后即可结束对话；下次启动说「开工」即可接续

## ⚠️ 注意事项

<!-- 坑、暂时 workaround、不要动的东西 -->
- 本专案刻意保留为「测试用」，不要把真实业务塞进来
- 当前环境**无 Obsidian MCP 工具**，L3 笔记更新靠 `write` 工具直接编辑 vault 内档案；新机器若无 MCP 可同样处理
- 路径 `E:/ai/teach-study/` 不在云端硬盘同步目录下，跨电脑搬运需手动
- `gh` CLI 没在 PATH，要用绝对路径 `/c/Program Files/GitHub CLI/gh.exe`
- Obsidian 装在非标准路径 `D:\hj\soft\tools\Obsidian\`，从 `C:\Users\Public\Desktop\Obsidian.lnk` 解析

## 🕐 最后更新

- 时间：2026-09-04 19:17
- 更新者：pi @ LAPTOP-KL01CRG6
- Git push：✅ 已推（commit `6748c6f` 已推至 GitHub `hujun1/test-project-0904`）