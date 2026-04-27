# 项目记忆

## 项目范围
- 当前工作区负责游戏原型与玩法验证，包含早期“割一波 / 生存割草”实验线，以及后续的 Claw / 幽塔术士卡牌子线。
- 联动项目仅保留业务关系：`C:\Users\chrisciou\WorkBuddy\20260413110256` 负责流量影片引流；两个项目严格分开处理，不继承彼此任务细节。

## 当前仍有效的协作约定
- 每次改完代码，默认同步更新 `README.md`、`docs/当前任务框架.md`、`.workbuddy/memory/MEMORY.md` 与当日日志。
- 代码或正式文档只要有值得保留的改动，就直接提交并推送到当前 GitHub 仓库，无需额外等待用户再提醒。
- 对外提供链接前必须先验证可访问；微信场景优先给根路径可达方案，并准备备用链接或附件兜底。
- 机制设计里要主动前置识别明显副作用，不要等用户指出后再补救。

## 技术与部署
- 主要技术栈：纯 HTML5 Canvas + 原生 JavaScript；无需构建工具，HTML 原型可直接打开。
- `claw/godot-v01/` 为 Godot Web 导出包，用于和 H5 原型做同题材对照验证。
- GitHub 仓库：`jojo780849/cut-them-all`
- GitHub Pages 主要入口：
  - `game.html`：远程射击旧主线
  - `demo_melee.html`：近战主线
  - `demo_ranged_bazaar.html`：纸扎夜市验证线
  - `demo_ranged_juice.html` / `juice.html`：远程爽感验证线
  - `b.html`：Claw H5 机制镜像
  - `claw/`、`claw/b.html`、`claw/h.html`、`claw/g.html`：Claw 竖版、镜像、横版与 Godot Web 入口

## 主要原型现状（精简版）
- `game.html`：远程射击版，已具备自动索敌射击、敌人追踪、成长系统与多阶段 Boss 战。
- `demo_melee.html`：当前割草近战主线，核心为“主近战 + 副远攻被动槽 + 单摇杆”，已完成三把主武器、专属升级树、打击感、Boss、无敌帧、回血掉落与 UI 收束。
- `demo_ranged_juice.html` / `juice.html`：远程爽感实验线，重点验证三把远程武器与 6 套 JUICE 反馈模块。
- `demo_ranged_bazaar.html`：纸扎夜市验证线，重点验证波次 / 商店 / 功德箱循环，以及可自动连跑的测试员。
- `merge_shot_mobile_demo.html` / `m.html` / `msd_v2_20260421.html`：拖拽瞄准 + 松手连珠 + 三色技能的低负担射击验证。
- `block_combat_mobile_demo.html`：拼块放置战斗验证线，用清线伤害和三色能量测试“低操作负担 + 空间策略”。
- `spire_fusion_mobile_demo.html` / `squad_demo.html` / `warlock_v0_1.html` / `warlock_v0_2.html`：竖版卡牌展示、小队指挥、术士出牌与召唤联动的前置验证组。
- `b.html`：已从旧 warlock 镜像演化为 `Claw 機制鏡像 v2.6`，聚焦双战流程、格挡→小鬼→主角承伤传导、召唤小鬼 / 使魔号令 / 联动卡闭环。
- `claw/index.html` / `claw/b.html`：幽塔·术士竖版正式版入口，已形成敌人职责化、意图说明、点按 inspect 与压制减能量表达。
- `claw/h.html`：同逻辑横版预览，用于布局与可读性对照。
- `claw/g.html` / `claw/godot-v01/index.html`：Godot Web 对照入口。

## 近期里程碑
- 2026-04-03：创建 MVP，并推进到天赋系统与 GitHub Pages 部署。
- 2026-04-17：近战主线集中推进到 V15，明确“主近战 + 副远攻被动槽”方案。
- 2026-04-18 ～ 2026-04-20：补齐远程爽感实验线与纸扎夜市自动测试员能力的正式文档记录。
- 2026-04-21：新增三条“降低操作负担”验证线：合球射击、拼块战斗、根路径兼容入口。
- 2026-04-22：新增竖版卡牌 / 小队指挥 / 术士联动验证组。
- 2026-04-26：补录 Claw / 幽塔术士 H5 + Godot Web 验证线，确认根目录 `b.html` 已切为 Claw 机制镜像，`claw/` 目录入口结构完成归档。
