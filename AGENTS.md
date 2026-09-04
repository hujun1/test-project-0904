# 测试专案技能使用（专案蓝图）

> 本档为跨 Agent 通用的专案蓝图（AGENTS.md 开放标准）。任何 Agent 的每个 session 都应先读本档＋`handoff.md`。

## 专案简介

本专案用于测试 `project-init`（专案初始化技能）能否正常在本机环境建立 L1 本地蓝图。本专案本身不承载真实业务逻辑，目的是验证 SOP 流程、档案格式与跨 Agent 互通性。

## 关键时程

<!-- 格式：- 事件名称：日期（说明）；没有就留白 -->

## 目标与路线图

<!-- 用 checklist 追踪，收工技能会更新这里 -->
- [ ] 阶段一：完成 L1 本地蓝图建立（AGENTS.md + handoff.md）
- [ ] 阶段二：测试 `startup` 技能（读 handoff.md 接续）
- [ ] 阶段三：测试 `shutdown` 技能（更新 handoff.md 并 git commit）
- [ ] 阶段四：补建 L2 / L3（如环境支援）

## 文件夹结构

<!-- 初始化时自动扫描生成，之后新增档案要更新 -->
```
test-project-0904/
├── .gitignore           # git 排除清单（L2）
├── AGENTS.md            # 专案蓝图（每个 session 都读）
├── handoff.md           # 交接档（开工读、收工写）
└── 专案工作流程.md       # Obsidian vault 详细笔记（L3）
```

## 同步层级（本专案初始化至第 3 层级）

| 层级 | 平台 | 位置 | 读取时机 |
|------|------|------|---------|
| L1 | 本地 | `AGENTS.md` ＋ `handoff.md` | 每个 session |
| L2 | GitHub | `hujun1/test-project-0904`（私有） | 指定时 |
| L3 | Obsidian | vault `E:\ai\teach-study` / `test-project-0904/专案工作流程.md` | 有需要时 |

## 工作约定

- 任何 Agent、任何电脑：**开工先读 `handoff.md`，收工必更新 `handoff.md`**
- 修改共用档案前先读最新内容，避免覆盖其他 Agent 的变更
- 所有回应与文件使用简体中文
- 修改前先确认计划，优先保留原有资料结构

## 安全与隐私（不可违反）

- **不把 API key、密码、凭证写进 repo**，也不要贴进 `AGENTS.md`／`handoff.md`；一律放 `.env` 并列入 `.gitignore`
- **学生资料只用座号**，不出现姓名、学号、班级以外的个资、照片或联络方式
- 要公开分享前，先确认档案里没有上述两类内容