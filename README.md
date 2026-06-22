# 游戏复刻 · 通用模板

一套可复用的游戏复刻模板,用于「导演 + 执行 AI(Claude Code)手写玩法逻辑」的工作流。与具体游戏无关,复刻任何游戏都可套用。

## 文件
- **[`kickoff-template.md`](./kickoff-template.md)** — 开工补充信息(配 runbook 用):只补「这一个游戏要复刻什么」(原作 + 核心循环 + 灵魂系统 + 参考),流程/纪律/建工程不重述,全走 runbook。
- **[`impl-card-template.md`](./impl-card-template.md)** — 玩法实施卡模板(导演 5 栏 + 执行 AI 回填 5 栏)+ 交活 Prompt + 里程碑拆分指引 + 小抄。
- **[`spec-template.md`](./spec-template.md)** — 真值规格(扒真值)骨架:硬真值 / 手感值 / API 契约 / 待确认。

## 用法
每复刻一个游戏:
1. 复制本套模板到该游戏工程的 `docs/`。
2. 把 `<游戏>`、`<系统>`、`<里程碑>` 等占位替换成该游戏的实际内容。
3. 按「最小可玩闭环 → 逐系统铺开(灵魂系统重点做)→ 打磨」的节奏,每个里程碑用 `impl-card-template.md` 填一张实施卡,交给执行 AI。
4. 真值统一扒进 `spec-template.md`(每个可量化系统一张表,每个值标 [HARD]/[FEEL]/[TODO] + 出处)。
