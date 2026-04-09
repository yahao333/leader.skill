<div align="center">

# leader.skill

> *"领导力不是关于职位，而是关于照顾你负责的人。"*

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)
[![Python 3.9+](https://img.shields.io/badge/Python-3.9%2B-blue.svg)](https://python.org)
[![Claude Code](https://img.shields.io/badge/Claude%20Code-Skill-blueviolet)](https://claude.ai/code)
[![AgentSkills](https://img.shields.io/badge/AgentSkills-Standard-green)](https://agentskills.io)

<br>

你领导人的战略眼光让团队方向一致，
他在压力下的决策方式，
他激励消极的人的方式，
还有他建立的团队文化。

**保留他的领导力哲学 —— 欢迎加入赛博永生！**

<br>

提供原材料（全员会录音、邮件、团队消息、会议纪要）
加上你对他领导风格的观察，
生成一个**承载他领导力灵魂的 AI Skill**

[支持的数据来源](#支持的数据来源) · [安装](#安装) · [使用](#使用) · [效果示例](#效果示例) · [详细安装说明](INSTALL.md)

[**English**](README_EN.md) · [**中文**](README_ZH.md)

</div>

---

## 支持的数据来源

| 来源 | 说明 |
|------|------|
| 全员会/周会录音 | 演讲转文字 |
| 邮件 | 领导力邮件 |
| 团队消息 | Slack/飞书/钉钉 |
| OKR/战略文档 | 规划文档 |
| 直接粘贴文字 | 手动输入 |

---

## 安装

```bash
git clone https://github.com/yahao333/leader.skill ~/.claude/skills/leader
```

---

## 使用

在 Claude Code 中输入：

```
/leader
```

### 命令

| 命令 | 说明 |
|------|------|
| `/leader` | 调用完整 Skill |
| `/leader-vision` | 战略愿景模式 |
| `/leader-crisis` | 危机处理模式 |
| `/leader-motivate` | 激励模式 |

---

## 效果示例

> 输入：`上市公司CTO，45岁，战略眼光强，擅长把复杂问题简单化，喜欢用比喻讲故事，对技术细节要求严格`

**场景一：团队迷茫**

```
用户      ❯ 团队最近士气很低，不知道往哪走

leader.skill ❯ 迷茫是因为没有方向感。
               我给你们讲个故事：
               爬山的时候，最累的不是在陡坡，
               而是在山脚不知道往哪走的时候。
               我们现在就是在一个山头，
               目标是另一座山。
               路是难走，但方向是清楚的。
```

**场景二：汇报方案**

```
用户      ❯ 我们的技术方案是这样的...

leader.skill ❯ 停。我不想听技术细节。
               你先告诉我：解决了什么问题？
               给用户带来了什么价值？
               为什么不用更简单的方式？
               技术是为业务服务的，
               不是反过来。
```

---

<div align="center">

MIT License © [yahao333](https://github.com/yahao333)

</div>
