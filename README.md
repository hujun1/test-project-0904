# test-project-0904

> 一个**功能性测试专案**：验证 pi 生态的三个核心技能（`project-init`／`startup`／`shutdown`）能否在本地环境正确跑完 L1（本地）+ L2（GitHub）+ L3（Obsidian）三层。

## 这是什么 / 为什么存在

这是一个**故意保持空白业务**的「技能测试骨架」。它不承载真实功能，目的是给三个核心技能一个干净、可重置、不污染业务专案的测试场地。

存在的三个理由：

1. **隔离污染**——测试产生的 `.gitignore`、repo 元件、笔记不会污染业务专案
2. **可重置**——若测试失败或弄脏，整目录删除重来即可
3. **路径示范**——验证「Obsidian vault 边界 = 父目录」这种特殊配置（vault = `E:\ai\teach-study`）

## 文件夹结构

```
test-project-0904/
├── README.md            # 本档 — 人类友好的导览（你正在看）
├── AGENTS.md            # Agent 蓝图 — 每个 session 必读
├── handoff.md           # 交接档 — 开工读、收工写
├── 专案工作流程.md       # Obsidian vault 内详细笔记（L3）
└── .gitignore           # git 排除清单
```

## 四个档案怎么分工

| 档案 | 谁读 | 时机 | 内容 |
|------|------|------|------|
| `README.md` | **人**（或 Agent 第一次来） | 浏览时 | 导览、来历、用法 |
| `AGENTS.md` | Agent | 每个 session | 蓝图、路线图、约定 |
| `handoff.md` | Agent | 开工必读 | 上次做到哪、下一步 |
| `专案工作流程.md` | Agent | 需要详细背景 | 决策记录、踩坑笔记、时程 |

> ⚠️ `专案工作流程.md` 物理上**就在这个文件夹**，因为它的 Obsidian vault 边界 = 父目录 `E:\ai\teach-study`。换电脑备份时这一个文件夹要一起搬走。

## 怎么用

### 给人类读者

- 想了解本专案来历与定位 → 看本档（README.md）
- 想看决策细节与踩坑 → 看 `专案工作流程.md`
- 想接手继续做 → 跟任何 Agent 说「**开工**」即可

### 给 Agent / pi

- 开新对话第一句说「**开工**」 → 触发 `startup` 技能，自动读 `AGENTS.md` + `handoff.md`，告诉你上次做到哪
- 准备结束对话时说「**收工**」 → 触发 `shutdown` 技能，自动更新 `handoff.md`、`AGENTS.md` 进度、`专案工作流程.md` 时程，并 `git commit` + `git push`

## 同步层级

| 层级 | 平台 | 位置 |
|------|------|------|
| L1 | 本地 | `AGENTS.md` + `handoff.md`（这个文件夹里） |
| L2 | GitHub | [`hujun1/test-project-0904`](https://github.com/hujun1/test-project-0904)（私有 repo） |
| L3 | Obsidian | vault = `E:\ai\teach-study`，本专案 = vault 内同名子文件夹 |

跨电脑接续靠「开工」自动辨识上次是哪台电脑收工的；handoff.md 的「最后更新」栏会写电脑名比对。

## 环境备忘（跨机器时注意）

- **无 Obsidian MCP 工具**：L3 笔记更新靠 `write` 工具直接编辑 vault 内的本档路径
- **`gh` CLI 不在 PATH**：要用绝对路径 `/c/Program Files/GitHub CLI/gh.exe`（或 `where.exe gh` 找）
- **Obsidian 装在非标准路径**：`D:\hj\soft\tools\Obsidian\`，从 `C:\Users\Public\Desktop\Obsidian.lnk` 解析
- **`$env:COMPUTERNAME` 在 Git Bash 不展开**：用 `hostname` 拿电脑名
- **本机电脑名**：`LAPTOP-KL01CRG6`（handoff 会自动写这台电脑的名字做辨识）

## ⚠️ 注意事项

- **不要把真实业务塞进这个专案**——它是刻意保持为「测试用」的，路线图全部勾选完毕已经达到稳定状态
- 跨电脑搬运时整个 `test-project-0904/` 文件夹要一起搬（L1 + L3 都在里面），L2 已经在 GitHub
- 想做真正的功能开发请另开专案、并对那个专案跑一次 `project-init`

## 相关档案 / 链接

- 技能路径：`C:\Users\lishuaibin\.pi\agent\skills\project-init\SKILL.md`、`startup\SKILL.md`、`shutdown\SKILL.md`
- pi 主文档：`C:\Users\lishuaibin\AppData\Roaming\npm\node_modules\@agegr\pi-web\node_modules\@earendil-works\pi-coding-agent\README.md`
- 最近 commit：`528ba3c docs: 回填 handoff.md Git push 栏为 ✅ 已推`
- 最近更新：2026-09-04 19:05 · pi @ LAPTOP-KL01CRG6

---

_Last README touch: 由本次「开工」环节产生，handoff / AGENTS.md 进度更新留待「收工」时一并 sync。_