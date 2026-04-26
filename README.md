# 割一波

## 项目定位
- 本项目：游戏项目，负责流量变现
- 联动项目：`C:\Users\chrisciou\WorkBuddy\20260413110256`
- 联动项目职责：流量影片引流
- 处理原则：两个项目严格区分开，不继承彼此的任务细节，只保留联动关系与职责分工

## 当前技术栈
- 纯 HTML5 Canvas + 原生 JavaScript 为主，另新增 `claw/godot-v01/` Godot Web 导出包用于同题材对照验证
- 多个单文件原型并行推进：`demo_melee.html` / `demo_ranged_bazaar.html` / `demo_ranged_juice.html` / `juice.html` / `merge_shot_mobile_demo.html` / `m.html` / `msd_v2_20260421.html` / `block_combat_mobile_demo.html` / `spire_fusion_mobile_demo.html` / `squad_demo.html` / `warlock_v0_1.html` / `warlock_v0_2.html` / `b.html` / `demo_ranged.html` / `game.html` / `claw/index.html` / `claw/b.html` / `claw/h.html`
- 分享与试玩入口同时保留根目录短链镜像（如 `juice.html` / `m.html` / `b.html`）与子目录正式入口（如 `claw/`）
- 无需构建工具，HTML 原型双击即可运行；`claw/godot-v01/` 为已导出的网页构建

## 跨电脑协作结构
- GitHub：代码、Excel 进度表、设计文档
- 腾讯文档：协作版进度追踪、讨论结论、待确认问题
- `.workbuddy/memory/`：项目上下文、关键结论、每日推进记录

## 当前关键文件
- `demo_melee.html`：**近战版主力开发线（当前最新 V15）**
- `demo_ranged_bazaar.html`：**纸扎夜市验证线（方案B，含夜市商店/功德箱循环与内建自动测试员）**
- `demo_ranged_juice.html`：**远程爽感实验线（V3，6 套 JUICE 系统 + 画面内错误诊断 overlay）**
- `juice.html`：`demo_ranged_juice.html` 的短路径镜像，方便外部分享与试玩
- `merge_shot_mobile_demo.html`：**移动合球射击实验线**，用拖拽瞄准 + 松手连珠来降低逐发瞄准负担
- `m.html`：`merge_shot_mobile_demo.html` 的短路径镜像，适合微信/手机端快速进入
- `msd_v2_20260421.html`：`merge_shot_mobile_demo.html` 的防缓存镜像，用于绕过旧缓存
- `block_combat_mobile_demo.html`：**Block Combat 放置战斗实验线**，用拼块清线 + 三色能量技能验证轻操作战斗
- `spire_fusion_mobile_demo.html`：**尖塔融合竖版验证线**，把“竖版舞台 + 美术预留 + 点按解说 + 拖拽出牌”揉成一张可讲解的移动端卡牌样机
- `squad_demo.html`：**小队指挥验证线（分支1）**，验证 3 格站位 + 角色牌/技能牌拖拽出牌的指挥感
- `warlock_v0_1.html`：**术士卡牌验证线 v0.1**，偏炉石式的出牌感对照样机
- `warlock_v0_2.html`：**术士卡牌验证线 v0.2**，主角居中 + 召唤物侧翼 + 联动卡动态注入的当前迭代版
- `b.html`：**Claw H5 机制镜像 v2.6**，根目录短链入口，主打双战流程、格挡→小鬼→主角的承伤传导，以及召唤物联动卡注入
- `claw/index.html`：**幽塔·术士 v0.6 竖版正式版**，三怪站位 + 召唤物 + 联动卡的主入口
- `claw/b.html`：`claw/index.html` 的主玩镜像入口，便于外发与手机试玩
- `claw/h.html`：**幽塔·术士横版预览**，用于验证横版构图与信息密度
- `claw/g.html`：Godot Web 短链入口，自动跳转到 `claw/godot-v01/index.html`
- `claw/godot-v01/index.html`：**Claw Godot Web 导出入口**
- `demo_ranged.html`：远程版基础验证线
- `game.html`：远程射击正式版旧主线
- `index.html`：根路径跳转页，当前默认跳到 `m.html`

- `割一波_玩法设计进度表.xlsx`：项目进度表
- `docs/当前任务框架.md`：当前待办框架与优先级
- `.workbuddy/memory/MEMORY.md`：长期项目记忆
- `.workbuddy/memory/YYYY-MM-DD.md`：每日推进记录


## 在线体验
- **近战版（主力）**：https://jojo780849.github.io/cut-them-all/demo_melee.html
- **纸扎夜市验证线**：https://jojo780849.github.io/cut-them-all/demo_ranged_bazaar.html
- **远程爽感实验线**：https://jojo780849.github.io/cut-them-all/demo_ranged_juice.html
- **远程爽感短路径**：https://jojo780849.github.io/cut-them-all/juice.html
- **Claw H5 机制镜像**：https://jojo780849.github.io/cut-them-all/b.html
- **Claw 竖版正式版**：https://jojo780849.github.io/cut-them-all/claw/
- **Claw 竖版主玩镜像**：https://jojo780849.github.io/cut-them-all/claw/b.html
- **Claw 横版预览**：https://jojo780849.github.io/cut-them-all/claw/h.html
- **Claw Godot Web 短链**：https://jojo780849.github.io/cut-them-all/claw/g.html
- **远程版旧主线**：https://jojo780849.github.io/cut-them-all/game.html

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

## 纸扎夜市验证线 (demo_ranged_bazaar)
- 远程武器 + 20 波战斗 + 波间夜市商店/功德箱循环的经济验证样机，用来观察“成长靠商店、不靠系统白送”的节奏是否成立
- 新增内建游戏测试员（方案2+）：可从开局面板直接自动跑局，顶部 HUD 会显示测试员状态、趣味分与当前迭代次数
- 测试员具备墙体排斥、卡墙脱困、敌人与子弹威胁评估、残血寻治疗/低压捡资源等行为，并会在局间按贴墙率、卡住率、承伤表现做参数微调
- 支持自动连跑重开，便于持续观察波次、商店与资源循环是否稳定；键盘 `T` 可切换测试员，`R` 可在启用后切换单局/连跑

## 移动合球射击实验线 (merge_shot_mobile_demo)
- 用来验证“逐发手动瞄准太累”时，是否改成拖曳瞄准、松手后同角度 16 连珠会更轻松
- 敌人带红/蓝/绿弱点；命中对应弱点会累计队列，凑到 3 个会触发红重击/斩杀、蓝全场冰缓、绿扩散弹幕
- `m.html` 与 `msd_v2_20260421.html` 为同内容镜像；`index.html` 默认跳到 `m.html`，兼容微信只打开根域名的场景

## Block Combat 放置战斗实验线 (block_combat_mobile_demo)
- 用 8x8 棋盘 + 3 手拼块，把 Block Blast 的“放置解题”改造成会反击的战斗循环
- 每放 3 次敌人推进或出手一次；清线负责主要伤害，红/蓝/绿能量分别给爆发、护盾、回血
- 支持点选/拖拽放置与落点预览，用来测试“轻操作 + 空间策略”能否成为主线操作骨架

## 尖塔融合竖版验证线 (spire_fusion_mobile_demo)
- 把尖塔式卡牌战斗压成手机竖版单屏，先验证“角色舞台可见 + 手牌拖拽出牌 + 解说层”能否同时成立
- 舞台预留敌我立绘区，点角色可看说明；拖牌到敌人/自己即可出牌，适合拿来讨论未来美术与信息层如何共存
- 当前定位偏“讲结构的展示样机”，不是正式战斗数值原型

## 小队指挥验证线 (squad_demo)
- 分支1 聚焦“你是指挥官，不是单角色本体”这一手感：3 格场位、角色牌上场、技能牌指定友军或敌人
- 已验证角色/技能/战术三类卡、拖拽目标提示、场上单位即时反馈，适合继续往职业宇宙或小队协同发展

## 术士卡牌验证线 (warlock_v0_1 / warlock_v0_2)
- `warlock_v0_1.html`：先做偏炉石式出牌感，对照传统“我方在下、敌方在上”的回合制卡牌触感
- `warlock_v0_2.html`：进一步改成构图 D，主角居中、召唤物站两侧，并在召唤时动态注入对应联动卡，验证“术士指挥召唤物”是否比纯单卡更有职业味

## Claw / 幽塔术士验证线 (b.html / claw/)
- `b.html`：根目录短链已演化为 **Claw H5 机制镜像 v2.6**，当前聚焦双战流程（小怪战 → Boss 战）、格挡→小鬼→主角的承伤传导，以及小鬼召唤 / 使魔号令 / 联动卡注入这套最小闭环
- `claw/index.html` / `claw/b.html`：竖版 **v0.6 三怪站位正式版**，已具备哨戒鬼差 / 缚魂纸偶 / 纸甲阴兵三类敌人职责化，包含 intent badge、点按 inspect、压制（下回合减能量）与自护等战术提示
- `claw/h.html`：横版预览入口，用同一套卡牌与敌人逻辑验证横版构图、信息密度与手牌可读性
- `claw/g.html` / `claw/godot-v01/index.html`：Godot Web 导出入口与短链，用来对照 H5 原型和 Godot 落地版的 UI / 战斗节奏差异

## 自动同步



- **代码改完自动推送**：每次修改代码后自动 git push 到 GitHub + 同步更新本地文档（README/MEMORY/当前任务框架），确保 OpenClaw 等外部工具能读到最新状态
- 已配置每日 22:00 的"游戏项目每日收尾同步"自动任务
- 目标：更新项目记忆、必要进度文档，并将有价值的成果同步到当前 GitHub 仓库

## 当前玩法推进顺序
1. 先攻克核心玩法与战斗模型
2. 再定局内节奏、局外成长与武器体系
3. 最后统一包装主题，并与流量影片内容联动
