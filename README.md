# EC-Brand Proposal

> **品牌方案提案**：一套面向中国市场广告、品牌与 Campaign 提案的人机共创 Skill。
>
> A human–AI co-creation Skill for brand and campaign proposals in China.

[中文](#中文) · [English](#english)

## 中文

**EC-Brand Proposal** 让 AI 参与 Brief 研究、客户答疑、策略与创意、Campaign、媒介、方案叙事和 PPT 生产流程。

它不是“输入一份 Brief，一次生成整套方案”的自动化模板。它通过研究、多轮讨论、阶段判断与连续上下文，逐步定义问题、比较路径并收敛复杂提案，把 AI 的研究、整理和发散能力，与人的经验、审美和关键判断结合起来。

默认使用中文研究、解释和共创；也支持英文或中英双语协作。

### 核心特点

- **研究驱动**：Brief 是客户当前的表达，不自动等于真实问题或唯一答案。先研究品牌、品类、生意、消费者与竞争环境，再判断问题和路径。
- **分阶段共创**：AI 负责研究、发散、比较与推荐；人补充内部信息，并在真正改变方向的节点进行判断。
- **连续上下文**：持续保留证据、客户答疑、已选方向、放弃原因、现实限制与未知，减少多轮协作中的前提丢失。
- **动态接入**：可以从 Brief、策略、创意、Campaign、媒介、逐页内容或 PPT 等任意阶段开始，只回补真正会影响结果的必要上游。

### 适合谁

- 希望把时间留给关键判断的策略、创意、品牌与媒介从业者；
- 希望理解研究、策略、创意、媒介与成案之间关系的使用者；
- 想把团队经验与 AI 的研究、整理和发散能力结合起来的团队。

> 更多有效输入 + 持续讨论 + 连续上下文 = 增强人的提案能力。

### 一键安装

```bash
npx -y skills add mabzhang/ec-brand-proposal --global --agent '*' --yes
```

安装完成后，请重新打开 Agent 或开始一个新对话。

### 让 Agent 代为安装

也可以直接对具备终端与联网权限的 Agent 说：

> 请从 https://github.com/mabzhang/ec-brand-proposal 安装 `ec-brand-proposal` Skill，完整保留 `SKILL.md`、`references/`、`agents/`、`evals/` 和 `assets/`，并全局启用。安装完成后，请告诉我是否需要重启 Agent 或开启新对话。

### 手动安装

克隆完整仓库：

```bash
git clone https://github.com/mabzhang/ec-brand-proposal.git
```

将完整的 `ec-brand-proposal` 文件夹放入所使用 Agent 的 Skills 目录。不同 Agent 的目录位置可能不同，请以对应产品文档为准。

不要只复制 `SKILL.md`；`references/`、`agents/`、`evals/` 和 `assets/` 也是完整 Skill 的组成部分。支持读取本地文件夹的 Agent，也可以直接读取整个仓库。

### 开始使用

准备 Brief、会议记录、客户答疑、现有方案或其他必要材料，并说明：

- 最终希望获得什么；
- 哪些内容已经确认；
- 哪些条件不能改变；
- 当前最希望讨论或推进到哪一步。

推荐启动语：

> 使用 `$ec-brand-proposal`，结合这份 Brief 和已有材料，与我共创这次提案。最终希望得到【交付物】；已经确认【已确认内容】；不能改变【限制条件】。

具体路由、阶段规则与完成检查见 [`SKILL.md`](./SKILL.md)。

### 能力边界

- 默认面向中国市场；涉及品牌、市场、消费者、渠道、平台规则等当前事实时，需要联网检索和来源验证。
- 不默认抓取小红书笔记或评论区；需要此类观察时，应由用户提供授权材料或人工观察结果。
- 可以发展 KV 概念、TVC 方向与文字脚本、事件营销方向和媒介 Roadmap，但不直接替代 KV 成图、拍摄制作、生产级分镜或完整事件执行。
- PPT/PDF 生产依赖当前 Agent 可用的工具、文件权限和已经确认的逐页内容。
- Skill 提供研究、推理、比较和共创框架，不替代客户内部信息、行业经验、审美判断与最终决策，也不保证特定商业结果。

## English

**EC-Brand Proposal** brings AI into brief research, client Q&A, strategy, creative development, campaign planning, media planning, proposal narrative, and the PPT production workflow.

It is not a one-shot generator that turns a brief into a complete proposal automatically. It uses research, iterative discussion, stage-based decisions, and persistent context to define the real problem, compare possible paths, and gradually build a complex proposal. The goal is to combine AI’s research, synthesis, and ideation capabilities with human experience, taste, and judgment.

Chinese is the default working language. English and bilingual collaboration are also supported.

### Core features

- **Research-led**: A brief is the client’s current framing, not automatically the real problem or the only valid answer. The Skill first examines the brand, category, business, consumers, and competitive environment.
- **Stage-based co-creation**: AI researches, explores, compares, and recommends. People contribute internal knowledge and decide at moments that materially change direction.
- **Context continuity**: Evidence, client answers, selected directions, rejected options, constraints, and unknowns remain available across multiple rounds.
- **Dynamic entry**: Start from a brief, strategy, creative idea, campaign, media plan, page-by-page narrative, or PPT. The Skill only reconstructs upstream context that can materially affect the result.

### Who it is for

- Strategists, creatives, brand marketers, and media professionals who want to spend more time on consequential decisions;
- People who want to understand how research, strategy, creative, media, and proposal development connect;
- Teams combining their own expertise with AI-assisted research, synthesis, and exploration.

> Better inputs + sustained discussion + continuous context = stronger human proposal capability.

### Quick install

```bash
npx -y skills add mabzhang/ec-brand-proposal --global --agent '*' --yes
```

After installation, restart your Agent or begin a new conversation.

### Ask an Agent to install it

> Install the `ec-brand-proposal` Skill from https://github.com/mabzhang/ec-brand-proposal. Preserve `SKILL.md`, `references/`, `agents/`, `evals/`, and `assets/`, and enable it globally. When finished, tell me whether I need to restart the Agent or start a new conversation.

### Manual installation

```bash
git clone https://github.com/mabzhang/ec-brand-proposal.git
```

Place the complete `ec-brand-proposal` folder in your Agent’s Skills directory. The exact directory depends on the Agent, so follow its product documentation.

Do not copy only `SKILL.md`. The `references/`, `agents/`, `evals/`, and `assets/` directories are part of the complete Skill.

### Getting started

Prepare the brief, meeting notes, client Q&A, current proposal, and any other relevant material. State the desired deliverable, confirmed decisions, non-negotiable constraints, and the stage you want to reach.

Suggested prompt:

> Use `$ec-brand-proposal` to co-create this proposal with me, based on the attached brief and existing materials. The final deliverable is 【deliverable】; confirmed decisions are 【confirmed items】; non-negotiable constraints are 【constraints】.

See [`SKILL.md`](./SKILL.md) for routing, stage rules, and completion checks.

### Scope and limitations

- The default research context is the Chinese market. Current claims about brands, markets, consumers, channels, or platform rules require live research and source verification.
- The Skill does not scrape Xiaohongshu posts or comments by default.
- It can develop KV concepts, TVC directions and text scripts, event-marketing directions, and media roadmaps, but it does not replace finished artwork, filming, production-ready storyboards, or complete event execution.
- PPT/PDF production depends on the tools, permissions, and approved page content available in the current Agent environment.
- The Skill supports research and decision-making; it does not replace internal business information, professional expertise, creative judgment, or final human approval, and it cannot guarantee business outcomes.

## 联系与定制 / Contact and customization

需要根据团队流程、品类知识、交付模板或工具链定制 Skill？扫描下方二维码联系 **Mab**，添加时请备注“Skill 定制”。

Need a version tailored to your team workflow, category knowledge, delivery templates, or toolchain? Scan the QR code to contact **Mab** on WeChat and mention “Skill customization”.

<img src="./assets/mab-wechat-contact.jpg" width="360" alt="Mab WeChat contact QR code">

## 作者与许可 / Author and license

作者与版权所有者 / Author and copyright holder：**Mab**

Copyright © 2026 Mab. All Rights Reserved.

作者识别码 / Author ID：`MAB-ECBP-2026`

使用、改编与再发布条款见 [`LICENSE`](./LICENSE)。

See [`LICENSE`](./LICENSE) for terms of use, modification, and redistribution.
