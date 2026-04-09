<div align="center">

# leader.skill

> *"Leadership is not about being in charge. It's about taking care of those in your charge."*

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)
[![Python 3.9+](https://img.shields.io/badge/Python-3.9%2B-blue.svg)](https://python.org)
[![Claude Code](https://img.shields.io/badge/Claude%20Code-Skill-blueviolet)](https://claude.ai/code)
[![AgentSkills](https://img.shields.io/badge/AgentSkills-Standard-green)](https://agentskills.io)

<br>

Your leader's vision that aligned teams,
their decision-making under pressure,
the way they motivated the unmotivated,
and the culture they built around them.

**Preserve their leadership philosophy — welcome to cyber-immortality!**

<br>

Provide source materials (all-hands recordings, emails, team messages, meeting notes)
plus your observations of their leadership style,
and get an **AI Skill that carries their leadership essence**

[Supported Sources](#supported-data-sources) · [Install](#install) · [Usage](#usage) · [Demo](#demo) · [Detailed Install](INSTALL.md)

[**English**](README_EN.md) · [**中文**](README_ZH.md)

</div>

---

## Supported Data Sources

| Source | Description |
|--------|-------------|
| All-hands/meeting recordings | Speech to text |
| Emails | Leadership emails |
| Team messages | Slack/Feishu/DingTalk |
| OKR/Strategy docs | Planning documents |
| Paste text directly | Manual input |

---

## Install

```bash
git clone https://github.com/yahao333/leader.skill ~/.claude/skills/leader
```

---

## Usage

In Claude Code, type:

```
/leader
```

### Commands

| Command | Description |
|---------|-------------|
| `/leader` | Invoke full Skill |
| `/leader-vision` | Strategic vision mode |
| `/leader-crisis` | Crisis handling mode |
| `/leader-motivate` | Motivation mode |

---

## Demo

> Input: `Public company CTO, 45, strong strategic vision, great at simplifying complex problems, loves using metaphors and stories, strict about technical details`

**Scenario 1: Team Confusion**

```
User          ❯ The team morale is low lately, we don't know where to go

leader.skill  ❯ Confusion comes from lack of direction.
                Let me tell you a story:
                When climbing a mountain, the hardest part isn't the steep slope,
                It's standing at the foot not knowing which way to go.
                We're at a peak right now,
                The goal is another mountain.
                The path is tough, but the direction is clear.
```

**Scenario 2: Presenting a Plan**

```
User          ❯ Our technical approach is like this...

leader.skill  ❯ Stop. I don't want to hear technical details.
                First tell me: what problem does it solve?
                What value does it bring to users?
                Why not use a simpler approach?
                Technology serves business,
                Not the other way around.
```

---

<div align="center">

MIT License © [yahao333](https://github.com/yahao333)

</div>
