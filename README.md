# 外贸项目决策与执行助手

> 系统内部 ID：`foreign-trade-project-os`。受 Codex Skill 命名规范限制，内部 ID 必须使用小写英文字母、数字和连字符；日常界面和中文触发词使用“外贸项目决策与执行助手”。

一个面向外贸项目的证据驱动型 Agent Skill。它不替代行业知识库，也不替你判断市场必然成功；它负责约束 AI 如何理解项目、控制范围、审查证据、做出决策和复盘纠偏。

## 适用于什么

- 市场、客户类型、产品线、渠道等尚未完成商业验证的外贸项目；
- 同时出现很多任务，需要识别单一核心约束和唯一第一优先级；
- 需要区分事实、用户确认、推断、假设和未知；
- 需要对重要方案执行 Planner–Red Team–Judge 决策；
- 需要周复盘、月度复盘、异常事件复盘和 Project Auditor 风险扫描；
- 需要把“看起来不错”转化为可观察的询价、报价、付费样品、订单或复购证据。

它同样可用于大多数小团队 B2B 出海项目，不限定国家、平台或产品品类。

## 不适用于什么

- 查询一个简单、确定的外贸知识点；
- 用 AI 代替律师、税务师、海关、检测机构或平台官方规则；
- 自动发送开发信、自动报价、自动承诺材料/交期/合规、自动签约或付款；
- 把市场规模、点赞、回复、竞品零售价或 AI 的信心当作商业成立证明；
- 同时启动多个市场、渠道和品牌项目却不设范围门槛。

## 公开 Skill 与私人项目状态必须分开

```text
公开仓库（本仓库）
  稳定方法、判断规则、复盘协议、空白模板
              ↓ 引用
私人项目仓库
  project-state、decision-log、真实客户、产品、成本和进度
```

本仓库不得提交真实客户名单、供应商报价、个人资料、账号、密钥、合同、未公开产品资料或其他动态项目事实。

## 仓库结构

```text
foreign-trade-project-os/
├── SKILL.md
├── agents/
│   └── openai.yaml
└── references/
    ├── project-state-template.md
    ├── decision-log-template.md
    ├── review-protocol.md
    └── market-selection-test-template.md

tests/
├── pressure-test-cases.md
└── pressure-test-results.md
```

没有 Shell、Hooks、自动执行脚本或第三方依赖。

## 安装

对 Codex 直接说：

> 请从 GitHub 仓库 `tuzituziyi-ship-it/foreign-trade-project-os` 安装 `foreign-trade-project-os` Skill，并在安装后验证 SKILL.md 与 agents/openai.yaml。

如果手动安装，把仓库中的 `foreign-trade-project-os` 文件夹复制到本机 Codex Skills 目录。安装后重新开始一个任务，让 Codex 重新载入 Skill 列表。

## 第一次使用

1. 在私人项目目录中，用 `references/project-state-template.md` 创建 `project-state.md`。
2. 用 `references/decision-log-template.md` 创建 `decision-log.md`。
3. 保留 `review-protocol.md`，并设定周/月复盘时间。
4. 最简中文用法：

> 用外贸项目助手：下一步做什么？

如果需要强制指定系统内部 ID，也可以说：

> 使用 `$foreign-trade-project-os`。先读取当前项目的 project-state.md 和 decision-log.md，区分事实/推断/假设/未知，找出单一核心约束，只给一个第一优先级。重要决策执行 Planner–Red Team–Judge，缺证据时给最低成本验证，不宣布商业假设成立。

## 日常使用示例

- “用外贸项目助手：继续青岛饰品项目。”
- “我又想到三个新市场，使用 Skill 判断是否进入当前 Scope。”
- “做本周复盘，只保留下周一个第一优先级。”
- “对这个美国优先方案做最强反方审查。”
- “跑一次 Project Auditor，先报告最高风险，不自动扩任务。”
- “现有证据够不够通过商业验证 Evidence Gate？”

## 证据边界

商业假设只有在预先定义的强证据出现后才能升级。默认强度从高到低为：付费订单/复购、付费样品、真实报价后的持续推进、具体选品与价格/MOQ/运费问题、可解释的有效回复。浏览量、点赞、笼统好评和市场规模只是弱信号或代理指标。

## 版本与同步规则

- 本公开仓库是稳定方法和结构的唯一来源（source of truth）。
- 结构性改动先更新本仓库，再更新已安装 Skill。
- 私人项目仓库只记录所使用的公开 Skill 版本，不把项目事实同步回本仓库。
- 动态事实只更新私人仓库；方法论变化才更新本仓库。
- 每次结构更新必须通过 `tests/pressure-test-cases.md`。

## 当前边界

这是决策与纠偏系统，不是主动唤醒的定时器。定期复盘需要飞书任务、日历或独立 Automation 触发；Skill 只规定触发后 AI 应如何工作。
