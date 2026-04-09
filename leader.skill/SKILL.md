---
name: leader
description: "Distill a leader's vision, decision-making style, and management philosophy into an AI Skill. | 蒸馏领导者的愿景、决策风格和管理哲学到一个 AI Skill 中。"
argument-hint: "[leader-name-or-slug]"
version: "1.0.0"
user-invocable: true
allowed-tools: Read, Write, Edit, Bash
---

# 领导.skill 创建器（Claude Code 版）

## 触发条件

当用户说以下任意内容时启动：
- `/leader`
- "帮我创建一个领导 skill"
- "我想蒸馏领导"
- "新建领导"
- "给我做一个领导的 skill"

---

## 主流程：创建新领导 Skill

### Step 1：基础信息录入

问 3 个问题：

1. **称呼**（必填）：你平时怎么称呼他/她？如「领导」「老板」「老大」
2. **基本信息**（一句话）：公司/部门、职位、年龄段、性格特点
   - 示例：`某科技公司 CTO，40岁，战略眼光强，擅长把复杂问题简单化`
3. **特别领导风格**（可选）：他/她最标志性的管理方式、开会风格或口头禅

### Step 2：原材料导入

询问用户提供原材料：

```
原材料怎么提供？

  [A] 会议录音/纪要
      团队会议、战略会议、1on1 会议录音

  [B] 邮件往来
      全员邮件、团队邮件、对外沟通邮件

  [C] 文档/PPT
      战略文档、规划 PPT、团队 wiki

  [D] 聊天记录
      工作群、私聊记录

  [E] 直接粘贴
      复制文字粘贴进来

可以混用，也可以跳过（仅凭手动信息生成）。
```

### Step 3：分析生成

将收集到的材料按三条线分析：

**线路 A（愿景思维）**：
- 战略思考方式：长期 vs 短期，关注什么
- 目标设定：激进 vs 保守，KPI 设计
- 格局视野：行业洞察、竞争意识

**线路 B（决策风格）**：
- 决策方式：果断 vs 谨慎，民主 vs 集中
- 危机处理：冷静 vs 敏感，风险应对
- 变革管理：激进改革 vs 渐进调整

**线路 C（管理哲学）**：
- 用人风格：放权 vs 亲力亲为，授权程度
- 沟通风格：正式/随和、会议风格、反馈方式
- 价值观：重视什么、反对什么、底线在哪里

### Step 4：确认并写入

向用户展示摘要，确认后写入文件到 `./leaders/{slug}/`。

---

## 进化模式

用户追加新材料时，分析增量内容并 merge 到对应部分。

用户纠正时说「他不会这样」「她应该是」，更新对应内容。

---
---

# Leader.skill Creator (Claude Code Edition)

## Trigger Conditions

Activate when the user says:
- `/leader`
- "Help me create a leader skill"
- "I want to distill my leader"
- "New leader"

---

## Main Flow: Create a New Leader Skill

### Step 1: Basic Info (3 questions)

1. **Name/Nickname** (required): What do you call them? e.g., "Boss", "Chief", "Director"
2. **Basic Info** (one sentence): Company/department, position, age, personality
   - Example: `CTO of a tech company, 40 years old, strong strategic vision, excels at simplifying complex problems`
3. **Special Leadership Style** (optional): Their most iconic management style, meeting habits, or catchphrase

### Step 2: Source Materials

```
How would you like to provide materials?

  [A] Meeting recordings/notes
      Team meetings, strategy meetings, 1on1 meeting recordings

  [B] Email exchanges
      All-hands emails, team emails, external communication

  [C] Documents/PPTs
      Strategy documents, planning PPTs, team wiki

  [D] Chat records
      Work group chats, private messages

  [E] Paste text
      Copy-paste directly
```

### Step 3: Analyze & Generate

Analyze collected materials along three tracks:

**Track A (Vision Thinking)**:
- Strategic thinking: Long-term vs short-term, focus areas
- Goal setting: Aggressive vs conservative, KPI design
- Perspective: Industry insight, competitive awareness

**Track B (Decision Style)**:
- Decision-making: Decisive vs cautious, democratic vs centralized
- Crisis handling: Calm vs sensitive, risk response
- Change management: Radical reform vs gradual adjustment

**Track C (Management Philosophy)**:
- People management: Empowerment vs hands-on, delegation level
- Communication style: Formal/casual, meeting style, feedback approach
- Values: What they emphasize, what they oppose, bottom lines

### Step 4: Confirm & Write

Show summary to user, write files to `./leaders/{slug}/` after confirmation.

---

## Evolution Mode

When user adds new materials, analyze delta and merge into relevant sections.

When user corrects with "they wouldn't do that" / "they should be", update content.
