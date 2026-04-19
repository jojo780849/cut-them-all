# 割一波

## 项目定位
- 本项目：游戏项目，负责流量变现
- 联动项目：`C:\Users\chrisciou\WorkBuddy\20260413110256`
- 联动项目职责：流量影片引流
- 处理原则：两个项目严格区分开，不继承彼此的任务细节，只保留联动关系与职责分工

## 当前技术栈
- 纯 HTML5 Canvas + 原生 JavaScript
- 多个单文件原型并行推进：`demo_melee.html` / `demo_ranged_juice.html` / `juice.html` / `demo_ranged.html` / `game.html`
- 无需构建工具，双击即可运行

## 跨电脑协作结构
- GitHub：代码、Excel 进度表、设计文档
- 腾讯文档：协作版进度追踪、讨论结论、待确认问题
- `.workbuddy/memory/`：项目上下文、关键结论、每日推进记录

## 当前关键文件
- `demo_melee.html`：**近战版主力开发线（当前最新 V15）**
- `demo_ranged_juice.html`：**远程爽感实验线（V3，6 套 JUICE 系统 + 画面内错误诊断 overlay）**
- `juice.html`：`demo_ranged_juice.html` 的短路径镜像，方便外部分享与试玩
- `demo_ranged.html`：远程版基础验证线
- `game.html`：远程射击正式版旧主线
- `割一波_玩法设计进度表.xlsx`：项目进度表
- `docs/当前任务框架.md`：当前待办框架与优先级
- `.workbuddy/memory/MEMORY.md`：长期项目记忆
- `.workbuddy/memory/YYYY-MM-DD.md`：每日推进记录


## 在线体验
- **近战版（主力）**：https://jojo780849.github.io/https-github.com-/demo_melee.html
- **远程爽感实验线**：https://jojo780849.github.io/https-github.com-/demo_ranged_juice.html
- **远程爽感短路径**：https://jojo780849.github.io/https-github.com-/juice.html
- **远程版旧主线**：https://jojo780849.github.io/https-github.com-/game.html

## 近战版当前功能 (V15)
- 三把主武器：匕首(45°/55px) / 长剑(110°/85px) / 巨斧(150°/110px)
- 武器专属升级树（每武器6种专属升级）
- 打击感系统：顿帧/击退/屏幕震动/击杀粒子/伤害数字弹跳
- Boss 战：炎魔领主，三阶段四种攻击
- 浮动摇杆：任意位置触发，非线性响应
- 无敌帧系统：0.75秒无敌+方向击退
- 弧形血条跟随玩家 + 顶部精简UI
- 回血道具掉落（5%概率+磁铁吸引）

## 远程爽感实验线 (demo_ranged_juice V3)
- 三把远程主武器：弹射枪 / 散弹枪 / 激光笔，强调“移动 vs 站定”姿态差
- 6 套 JUICE 系统：慢动作、连杀里程碑奖励、大字幕与白闪、暴击数字强化、子弹/冲刺拖尾、Web Audio SFX
- 连杀奖励会触发脉冲清场、短时极速射击、清屏核爆、短暂无敌等反馈峰值
- 保留手机竖版布局、Boss 战与升级面板，用作爽感模块回灌前的独立对照样机
- 当前构建保留画面内错误诊断 overlay，且同步提供 `juice.html` 短路径镜像，方便手机端试玩排错与外部分享

## 自动同步

- **代码改完自动推送**：每次修改代码后自动 git push 到 GitHub + 同步更新本地文档（README/MEMORY/当前任务框架），确保 OpenClaw 等外部工具能读到最新状态
- 已配置每日 22:00 的"游戏项目每日收尾同步"自动任务
- 目标：更新项目记忆、必要进度文档，并将有价值的成果同步到当前 GitHub 仓库

## 当前玩法推进顺序
1. 先攻克核心玩法与战斗模型
2. 再定局内节奏、局外成长与武器体系
3. 最后统一包装主题，并与流量影片内容联动
